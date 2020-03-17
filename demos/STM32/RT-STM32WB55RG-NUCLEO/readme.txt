*****************************************************************************
** ChibiOS/RT port for ARM-Cortex-M4 STM32WB55RG.                          **
*****************************************************************************

** TARGET **

The demo runs on an STM32 Nucleo-WB55 board.

** The Demo **

The demo starts the "blinker" thread which unconditionally toggles LED_1 and
conditionally two other LEDs, LED_2 and LED_3, if two buttons are pressed, SW2
and SW3 respectively, in a forever loop. The "main" thread in a forever loop
checks SW1 and runs the test procedure if it is pressed. The test produces
outputs on the serial port SD1 (USART1, mapped on STLink v2-1 Virtual COM
Port).

** Build Procedure **

The demo has been tested by using the free Codesourcery GCC-based toolchain
and YAGARTO. just modify the TRGT line in the makefile in order to use
different GCC toolchains.

** Notes **

Some files used by the demo are not part of ChibiOS/RT but are copyright of
ST Microelectronics and are licensed under a different license.
Also note that not all the files present in the ST library are distributed
with ChibiOS/RT, you can find the whole library on the ST web site:

                             http://www.st.com
