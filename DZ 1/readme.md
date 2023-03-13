
# Настройка коммутатора

## Задачи:
### Ч1. Проверям настройки SW1 по умолчанию
### Ч2. Настройка основных параметров
    настройка SW1
    настройка PC-A (к порту F0/6)
### Ч.3 Проверка сетевых подключений 
    конфигурация устройства
    протестировать сквозное соединение (эхо-запрос)
    протестировать SSH, Telnet

## Схема подключения (сети)

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_1.png)
   
   1. Коммутатор SW1 подключается консольным кабелем к ПК
   2. С помощью PuTTY получаем доступ к SW1 (в packet tracer через консоль)


## Ч1. Смотрим настройки SW1 

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_2.png)

## Смотрим конфиг (ссылка на конфиг) (конфиг выгружен из SW1)
[![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_3.1.png)](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/Config%201/Sw1_running-config.txt)

(можно поменять конфиг в txt и сохранить, тогда конфигурация будет готовой)




 Вводим каманду enable (вход с правами root, привилегированный режим)
![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_4.png)

 И проверяем конфигурацию по умолчанию командой show running-config
 
 Проверяем свойства FastEthernet порта куда подключен ПК командой show interface f0/6

 ![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_5.png)

Просматриваем содержимое флеш памяти

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_6.png)

## Ч2. Настройка базовых параметров устройств 

# Задаем имя устройству

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_8.png)

# Создаем пароль для (config-line) 

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_9.png)

# Создаем пароль для (config)

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_10.png)

# Проверяем

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_11.png)

# Открываем VTY 

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_12.png)

# Создаем баннер

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_13.png)

# Сохраняем конфиг в стартовый конфиг 

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_14.png)

# Задаем ip адрес и открываем порты.

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%201/DZ%201%20JPG/Screenshot_15.png)
