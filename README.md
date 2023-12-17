# dear_imgui_generator

## Generate cimgui bindings
Go into the `dear_bindings` directory and run `python .\dear_bindings.py -o cimgui ..\imgui\imgui.h`, this will produce the necessary cimgui.h and cimgui.cpp files.

## Generate cimgui backends bindings
For generating the bindings for the backends the `imconfig.h` needs to be placed into the `backends` directory.
Then for generating the backend bindings run `python dear_bindings.py --backend -o cimgui_impl_opengl3 ..\imgui\backends\imgui_impl_opengl3.h` instead, 
this is specifically for the opengl3 bindings. Swap it out for what you need, e.g. `python dear_bindings.py --backend -o cimgui_impl_sdl2 ..\imgui\backends\imgui_impl_sdl2.h`
