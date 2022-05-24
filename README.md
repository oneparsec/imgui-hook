# imgui-hook
ImGui hook by matcool with extra additions. I created it to use as a submodule in the GDMM.

# How to use it?

First of all, you should create main rendering function, where you can put `ImGui::Begin("Window Title")` and stuff like that.
To set rendering function, call a `ImGuiHook::setRenderFunction(<YOUR-RENDER-FUNCTION-NAME>)`.

Then, if you want to, you can create initialization function. It will run only one time, on the program startup. It could be used for style and font applying.
To set init function, call a `ImGuiHook::setInitFunction(<YOUR-INIT-FUNCTION-NAME>)`.

Also, you can set key to show window using `ImGuiHook::setToggleKey(<VIRTUAL-KEY-CODE>)` to [set a key](https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes) and use `ImGuiHook::setToggleCallback([]() {<WHATEVER-YOU-WANT-TO-DO>});`.
