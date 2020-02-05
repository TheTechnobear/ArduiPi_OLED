project(arduiPi_OLED)

add_library(arduiPi_OLED
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
target_include_directories(arduiPi_OLED PUBLIC .)
set_target_properties(arduiPi_OLED PROPERTIES WINDOWS_EXPORT_ALL_SYMBOLS true)

