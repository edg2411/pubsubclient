# The component's registration file.
cmake_minimum_required(VERSION 3.5)

# Use idf_component_register to define the component's properties.
# This is the modern, recommended approach for ESP-IDF.
idf_component_register(
    # List all source files relative to this CMakeLists.txt file.
    SRCS "src/PubSubClient.cpp"
    
    # List the directories to add to the include path.
    # "src" makes `#include "PubSubClient.h"` work.
    INCLUDE_DIRS "src"

    # Define the component's dependencies.
    # This ensures the 'arduino' component is available and linked.
    REQUIRES arduino-esp32
)
