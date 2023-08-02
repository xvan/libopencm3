add_library(opencm3_STM32F1 STATIC 
    lib/stm32/f1/adc.c
    lib/stm32/f1/rtc.c
    lib/stm32/f1/timer.c
    lib/stm32/f1/rcc.c
    lib/stm32/f1/flash.c
    lib/stm32/f1/i2c.c
    lib/stm32/f1/gpio.c
    lib/stm32/common/dma_common_l1f013.c
    lib/stm32/common/exti_common_all.c
    lib/stm32/common/timer_common_all.c
    lib/stm32/common/spi_common_v1.c
    lib/stm32/common/flash_common_f01.c
    lib/stm32/common/usart_common_f124.c
    lib/stm32/common/dac_common_all.c
    lib/stm32/common/flash_common_all.c
    lib/stm32/common/st_usbfs_core.c
    lib/stm32/common/pwr_common_v1.c
    lib/stm32/common/gpio_common_all.c
    lib/stm32/common/rcc_common_all.c
    lib/stm32/common/desig_common_v1.c
    lib/stm32/common/dac_common_v1.c
    lib/stm32/common/adc_common_v1.c
    lib/stm32/common/usart_common_all.c
    lib/stm32/common/flash_common_f.c
    lib/stm32/common/iwdg_common_all.c
    lib/stm32/common/i2c_common_v1.c
    lib/stm32/common/desig_common_all.c
    lib/stm32/common/crc_common_all.c
    lib/stm32/common/spi_common_all.c
    lib/cm3/assert.c
    lib/cm3/dwt.c
    lib/cm3/nvic.c
    lib/cm3/scb.c
    lib/cm3/sync.c
    lib/cm3/systick.c
    lib/cm3/vector.c
    
    
    lib/usb/usb.c
    
    lib/usb/usb_dwc_common.c
    lib/usb/usb_dwc_common.h
    lib/usb/usb_control.c
    lib/usb/usb_standard.c
    lib/usb/usb_msc.c
    lib/usb/usb_private.h
    lib/usb/usb_f107.c
    lib/usb/usb_midi.c
    lib/usb/usb_hid.c

    lib/usb/usb_audio.c
    lib/usb/usb_cdc.c

    lib/stm32/can.c
    lib/stm32/st_usbfs_v1.c
)

target_compile_options(opencm3_STM32F1 PRIVATE
    -Wextra
    -Wimplicit-function-declaration
    -Wmissing-prototypes
    -Wredundant-decls                                      
    -Wshadow                                      
    -Wstrict-prototypes
    -Wundef
    -Wno-packed
)