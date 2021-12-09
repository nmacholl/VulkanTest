# Vulkan Test

This is a reproduction of the [Vulkan Test](https://vulkan-tutorial.com/Development_environment) tutorial built with SCons on Apple silicon. This repository can be used as a reference for anyone who wishes to get the VulkanSDK running on the new MacOS ARM architecture.

## Dependencies

The dependencies are the same as the official tutorial with the addition of SCons as a quick build system.

Note that for Apple silicon homebrew installs packages to `/opt/homebrew/` instead of `/usr/local/` on Intel based Macs. The SConstruct is already configured to use the former for glfw and glm.

## Building

The demo can be built by running `scons` in the repository root.
