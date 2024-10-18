# Stm32BasicDemo

This repos contains a very basic demo for a stm32, based on a NUCLEO-G070RB board.

The code implements:
- Blinking of the internal green led at 1Hz
- Reading of ADC1 IN0 for control of of an external led
- ADC1 is configured in DMA, continuous conversion mode and DMA continuous request
- The led is controlled based on PWM generated with timer 1 in center aligned mode 1
- The value of the ADC is used to set the PWM duty cycle (TIM1->CCR1)
- Reading of an i2c sensor (BME280) using code provided by sheinz (https://github.com/sheinz)

The code provided here come without any warranty. The solutions used to implement
the different functions are working but maybe not optimals and can contains bug.

Enjoy at your own risks!