# envtool
Ｄescription:
  Shell script tool envtool is used in Chromium chroot ENV.

Usage:
  ./envtool ${COMMAND} ${BOARD}
  1. ${COMMAND} must in COMMAND_LIST and ${BOARD} must in BOARD_LIST
     It's free for you to expand command handle and board in envtool script.
  2. First use in chroot ENV, please run `envtool ${COMMAND} ${BOARD}` once in chroot ENV.
     Which will create ~/trunk/image/${BOARD}* and ~/trunk/firmware/${BOARD}*.
     Then you can put image and firmware binary file in these paths.
     When you run `ectool flash_* ${BOARD}`, will flash firmware binary file from ~/trunk/firmware/${BOARD} automatically．

     
     
