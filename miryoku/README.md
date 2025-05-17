# Personal Build

## Flashing

To flash, run the [build-personal.yml](../.github/workflows/build-personal.yml) github action which will generate a
left and right version of the firmware. Then, to flash onto the keyboard, do the following:

1. Plug in your nice!nano to your computer.
2. Enter the bootloader by double-tapping the reset button.
3. Drag and drop the .uf2 file onto the NICENANO drive or copy it with your terminal.
4. After flashing is complete, the drive will disappear and the nice!nano will reboot.
   > _Note_: Your computer may report an error when transferring the file, you can likely ignore this.1
5. If you haven't yet, you can turn the power switch on by pushing it up on the side of the keyboard.

## Updating

All personal overrides are defined in [custom_config.h](./custom_config.h). Make any changes to keybindings in that
file.

## Config

Config variables need to be defined in the kconfig section of the [build-personal.yml](../.github/workflows/build-personal.yml)

## Deleting Existing Bluetooth Profiles

To delete a bluetooth profile, simply hold SHIFT while selecting the bluetooth profile number. More details in [this](https://www.reddit.com/r/ErgoMechKeyboards/comments/xc2c74/comment/io40uub/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button) post.
