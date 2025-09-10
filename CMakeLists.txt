# The component's registration file.
cmake_minimum_required(VERSION 3.5)

# This tells CMake to look for another CMakeLists.txt in the 'src' directory
# and process it. The sources and include directories will be defined there.
add_subdirectory(src)

# Define the component's dependencies. This ensures the 'arduino' component
# is available and linked.
set(COMPONENT_REQUIRES arduino)

# Register the component with the ESP-IDF build system.
register_component()
