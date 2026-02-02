# STM32 SP26 Workshop 1: Intro to STM32

Installation for STM32CubeIDE:
[ST Microelectronics software installation](https://www.st.com/en/development-tools/stm32cubeide.html)

F411RE basic details and **pinout**:
[NUCLEO-F411RE](https://os.mbed.com/platforms/ST-Nucleo-F411RE/)

***In order to use the printf() function your code => IT IS CRUCIAL THAT YOU DO THIS***
```C
int _write(int file, char* ptr, int len) {
	for(int i = 0; i < len; i++) {
		ITM_SendChar((*ptr++));
	}
	return len;
}
```

_Links for more resources_:

* [**F411RE reference manual**](https://www.st.com/resource/en/reference_manual/rm0383-stm32f411xce-advanced-armbased-32bit-mcus-stmicroelectronics.pdf)
* [**F4 family HAL documentation**](https://www.st.com/resource/en/user_manual/um1725-description-of-stm32f4-hal-and-lowlayer-drivers-stmicroelectronics.pdf)
