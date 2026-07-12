# Microproject #1 - Bidirectional LED Bit Shift Register

## Board
STM32F103C8T6 Bluepill

## IDE
STM32CubeIDE

## LEDs
PA0 - PA7

## Buttons
PB14 - Rotate Left
PB15 - Rotate Right

## Features
- Interrupt-driven using EXTI
- HAL GPIO functions
- Circular left/right bit rotation
- No polling in while(1)

## NVIC
EXTI15_10_IRQn enabled
Priority: 0
Sub Priority: 0

## Initial Pattern
00000001