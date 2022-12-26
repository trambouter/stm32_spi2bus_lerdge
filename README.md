# Конвертор SPI для дисплея Lerdge на st7796s

[Описание и подключение](https://github.com/trambouter/fb_st7796s_lerdge)

# Что понадобится
[VSCode](https://code.visualstudio.com/)

[PlatformIO](https://platformio.org/)

# Установка

Открываем проект в PlatformIO и компилируем.

# Заливка прошивки

По умолчанию используется протокол stlink для заливки прошивки в контроллер.

Можно залить прошивку и через USB-Uart, [Почитать тут](https://istarik.ru/blog/stm32/111.html)


# Разгон stm32

В файле main.c находим RCC_PLL_MUL9 - и меняем на RCC_PLL_MUL14 (112мгц) или RCC_PLL_MUL16 (124мгц).

