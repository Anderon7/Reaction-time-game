# Reaction-time-game
from pitop import Pitop, Button, LED, SoundSensor, LightSensor, UltrasonicSensor
from time import sleep

pitop = Pitop()
screen = pitop.miniscreen
led_red = LED("D0")
led_green = LED("D1")
btn = Button("D2")
sound_sensor = SoundSensor("D3")
dist_sensor = UltrasonicSensor("A0")
light_sensor = LightSensor("A1")

# start in the idle state
toggle_active = False
screen.display_text("IDLE")
while not screen.cancel_button.is_pressed:
    #system, is not active and button has been pressed
    if btn.is_pressed:
        # change states
        screen.display_text("ACTIVE")
        led_green.on()
        sleep(.5)
        toggle_active = True


    if toggle_active:
        light = light_sensor.reading
        distance = dist_sensor.distance
        sound = sound_sensor

        if distance < .2 or light < 30:
            led_red.on()
            led_green.off()
            screen.display_text("ALARM")
        else:
            screen.display_text("ACTIVE")
            led_red.off()
        sleep(.5)
max = 70
baby = False
if baby:
    max = max/2

while not screen.cancel_button.is_pressed:

    s = sound_sensor.reading
    if s > max:
        led_red.on()
        led_green.off()
        screen.display_text("ALARM")
    else:
        screen.display_text("ACTIVE")
        led_red.off()

    sleep(.1)
