# cs32f103-bluepill-quickstart

Since ST create a lot of barriers and obstacles for STM32 chinese clones development (clone stlink dongle + cs32f1 bluepill), one cannot benefit from ST provided mainstream STM32CubeIDE + one click ready to use gdb debugger with Eclipse frontend + integrated CubeMX. I experimented with a lot of ways to find the easiest + fastest way to working with STM32 chinese clones. This is the way that I found.

## Pros
- Smarter code linting thanks to `"ms-vscode.cpptools"` extension
- Far quicker startup time thanks to VSCode's lightweight
- Enable boilerplate code generation thanks to CubeMX
- Enable interactive debug using `"marus25.cortex-debug"`
- 

## Installing dependencies

- [XPack openocd](https://xpack.github.io/dev-tools/openocd/)
- [arm-none-eabi-*](https://developer.arm.com/downloads/-/gnu-rm)
- [VSCode extension "marus25.cortex-debug"](https://marketplace.visualstudio.com/items?itemName=marus25.cortex-debug)


After build the executable, (`make -j(nproc --all)`) and fix every hardcoded path, you should be able to open VSCode and start debugging right away.

You can open .mxproject to reconfigure and regenerate code as expected.