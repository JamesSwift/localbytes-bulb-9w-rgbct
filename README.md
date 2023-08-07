# Local Bytes Smart Bulb - 9w RGB+CT
ESPHome configuration for the <a href="https://www.mylocalbytes.com/products/smart-bulb-9w-rgbct">local bytes rgbct smart light bulb</a>, with support for color correction.

![Capture+_2023-08-07-19-14-27](https://github.com/JamesSwift/localbytes-bulb-9w-rgbct/assets/2080205/37edc3af-0707-4691-892a-eae50c8ebfad)


It's described as a RGB+CT, but in reality its a RGBWW.

If flashing on top of the factory suplied Tasmota firmware, you will receive an error that there is not enough space. In that case, flash the minimal firmware first, connect to the wifi hotspot it creates, then flash the full firmware.

To color correct the bulb, the procedure I use is to switch to RGB mode in home assistant and choose the white center of the color wheel (so that the red, green, and blue LEDs are being used to make white light). The color produced at this point is normally not a very "white" white. I then move the "Max Power" sliders until the bulb appears as white as possible. I then try choosing different colors on the color wheel and make some small tweaks if needed.
