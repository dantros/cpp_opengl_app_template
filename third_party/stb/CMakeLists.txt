
add_library(stb_image STATIC
    "stb_image.cpp"
    "stb_image.h"
    "stb_image_resize2.h"
    "stb_image_write.h"
)
set_property(TARGET stb_image PROPERTY CXX_STANDARD 11)