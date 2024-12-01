# New Keyboard Shield

ZMK 公式に倣って動かしてみることを目的とする。
keyboard_name は`my_keyboard`とする。
今回は Unibody で作成する。

必要ファイルを作成

```
mkdir boards/shields/my_keyboard
touch boards/shields/my_keyboard/Kconfig.shield
touch boards/shields/my_keyboard/Kconfig.defconfig
touch boards/shields/my_keyboard/my_keyboard.overlay
touch boards/shields/my_keyboard/my_keyboard-layouts.dtsi
touch boards/shields/my_keyboard/my_keyboard.keymap
touch boards/shields/my_keyboard/my_keyboard.zmk.yml
```

... 実装

ビルド

```
west build -b my_keyboard
> usage: west [-h] [-z ZEPHYR_BASE] [-v] [-q] [-V] <command> ...
> west: unknown command "build"; do you need to run this inside a workspace?

# なんかエラー出たからinit試してみる    https://zmk.dev/docs/development/local-toolchain/setup/native
west init
> FATAL ERROR: target directory already exists (/Users/igusaya/Develop/Study/keyboard/my-shield-module/zephyr)
```
