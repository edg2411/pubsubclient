# Minimum CMake version required
cmake_minimum_required(VERSION 3.5)

# Set the component name (must match directory name in ESP-IDF components folder)
set(COMPONENT_SRCS 
    src/PubSubClient.cpp
)
set(COMPONENT_ADD_INCLUDEDIRS 
    src
    .
)

# Link to Arduino core (provided by ESP-IDF Arduino as a component)
set(COMPONENT_REQUIRES arduino)

register_component()
