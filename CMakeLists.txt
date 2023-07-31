add_library(STM32F1 STATIC 
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
)

target_include_directories(STM32F1 PUBLIC
    include
)

target_compile_definitions(STM32F1 PUBLIC
    -DSTM32F1
)

target_compile_options(STM32F1 PRIVATE
    -Wextra
    -Wimplicit-function-declaration
    -Wmissing-prototypes
    -Wredundant-decls                                      
    -Wshadow                                      
    -Wstrict-prototypes
    -Wundef
)