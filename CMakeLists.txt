cmake_minimum_required(VERSION 3.5)
set ( ESP_IDF_SSD1306_SRCS
      "components/ssd1306/ssd1306_i2c.c"
      "components/ssd1306/ssd1306_spi.c"
      "components/ssd1306/ssd1306.c"
) 
idf_component_register(SRCS ${ESP_IDF_SSD1306_SRCS}
                    INCLUDE_DIRS "components/ssd1306/."
                    REQUIRES "driver" 
                    )

project(esp-idf-ssd1306)