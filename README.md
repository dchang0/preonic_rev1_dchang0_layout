# preonic_rev1_dchang0_layout

A custom QMK layout/keymap for the Preonic Rev. 1 ortholinear keyboard.

Place the `dchang0_rev1` folder and its contents in your `qmk_firmware/keyboards/preonic/keymaps` folder and build and flash it using the following command:

```
make preonic/rev1:dchang0_rev1:dfu
```
Remember to push the RESET button on the bottom of the Preonic before the flashing utility times out.

Note that this layout can work unmodified with the Preonic Rev. 2. For the Preonic Rev. 3, it will work, but it does not have the additional RGB LED backlight controller keys that should be on the Adjust layer.

For more details on the differences from the default layout, check out the dchang0_rev1/readme.md file.
