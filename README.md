# stm32_nucleo

This repo is created to keep track of the progress made on the STM32 NUCLEOF446ZE microcontroller board

Also this is my first git project, so a way to learn how to do things on the git

#LED_ON_OFF

This is the first experiment I have done with STM32 NUCLOEF446ZE board and as every begineer, I started with LED blinking.

The link for LED blinking video is:
https://drive.google.com/file/d/13lHSLajm96ROopDcOErPAtRRd88vsoF_/view?usp=sharing


#code description

The code is written in main.c file in the while loop where the user code section is mentioned and defined as 
  /* USER CODE BEGIN WHILE */
  /* USER CODE END WHILE */

The LED is tuned on by writing on the pin that is connected to the LED, in this case it is PB0. The write syntax is found in stm32f4xx_hal_gpio.c file as is:
  //HAL_GPIO_WritePin(GPIO_TypeDef* GPIOx, uint16_t GPIO_Pin, GPIO_PinState PinState)
A delay of 1s is given after the LED ON and OFF to see the difference clearly
  //HAL_Delay()

