project(arduiPi_OLED)


add_library(arduiPi_OLED SHARED
	Adafruit_GFX.cpp
	ArduiPi_OLED.cpp
	Wrapper.cpp
	bcm2835.c
	glcdfont.c
	Adafruit_GFX.h
	ArduiPi_OLED.h
	ArduiPi_OLED_lib.h
	bcm2835.h
        )
target_link_libraries(arduiPi_OLED i2c)
target_include_directories(arduiPi_OLED PUBLIC .)
