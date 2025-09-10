# This file defines the build properties for the component's source code.

# Set the source files to be compiled for the component.
set(COMPONENT_SRCS
    "PubSubClient.cpp"
)

# Set the directory that contains the public header files.
# In this case, the 'src' directory itself contains 'PubSubClient.h'.
# This makes it available to other components that depend on it.
set(COMPONENT_ADD_INCLUDEDIRS ".")
