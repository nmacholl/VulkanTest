"""SConstruct for VulkanTest
To build run:
    $ scons
"""

vulkan_environment = Environment(
    CPPPATH=["/opt/homebrew/include/"],
    LIBS=["libglfw","libvulkan"],
    LIBPATH=["/usr/local/lib", "/opt/homebrew/lib/"],
    tools=["default", "clangxx"],
    VK_ICD_FILENAMES = "vulkansdk/macOS/share/vulkan/icd.d/MoltenVK_icd.json",
    VK_LAYER_PATH = "vulkansdk/macOS/share/vulkan/explicit_layer.d",
)

# This is not a serious project, always build a debug binary.
vulkan_environment.Append(CCFLAGS=["-g", "-O0"])

vulkan_environment.Program(target="#/bin/VulkanTest", source="#/src/main.cpp")