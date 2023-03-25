# Просмотр таблицы MAC адресов

## Задачи:
### Ч1. Создание и настройка сети согласно условиям ТЗ
### Ч2. Изучение таблицы MAC адресов
    
## Схема подключения (сети)

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.0.png)
   
# Ч1. Выставляем и прописываем на устройствах базовые параметры: имена хостов, IP адреса, password и тд. Согласно приведенной схеме.

 | Устройство | интерфейс |   IP адрес     |      Маска      |
 |------------|-----------|----------------|-----------------|
 |     SW1    |   VLAN 1  |  192.168.1.11  |  255.255.255.0  |
 |     SW2    |   VLAN 1  |  192.168.1.12  |  255.255.255.0  |
 |    PC-A    |     NIC   |  192.168.1.1   |  255.255.255.0  |
 |    PC-B    |     NIC   |  192.168.1.2   |  255.255.255.0  |
 
 
 
 ![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.1.png)


# Ч2. Таблица MAC адресов коммутатора

# Ш.1.a  При просмотре адаптера PC-A и PC-B, с помощью утилиты ipconfig /all наблюдаем следующие физические адреса 

 ![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.3.png)
 
  | Устройство |        адрес           |  
  |------------|------------------------|
  |     PC-A   |    0002.1755.36E2      | 
  |     PC-B   |    0005.5E64.4C58      |
 
# Ш.1.b  Смотрим данные коммутаторов с помощью команды show interface f0/1 на каждом коммутаторе
 
 ![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.2.2.png)
 
  | Устройство |         адрес         |  
  |------------|-----------------------|
  |     SW1    |     0003.e419.d701    | 
  |     SW2    |     0040.0b9d.a501    | 
 
 # Ш.2.a Подключаемся через консольный кабель к коммутатору SW2 
 
 # Ш.2.b Просматриваем таблицу MAC адресов с помощью команды show mac address-table 

 # сравниваем данные таблицы MAC и данные порта.

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.7.png)

 # Ш.3.a-b Очищаем таблицу MAC на SW2 командой clear mac address-table

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.8.png)

# Ш.3.a-c С PC-B отправляем эхо запросs на устройства в сети и смотрим таблицу MAC 

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.9.png)

![](https://github.com/Grotemast/STUDIES/blob/main/DZ%202/DZ%202%20PNG/Screenshot_2.10.png)

# Как видим что все устройства распознаны по MAC адресам.

# Полный список MAC (физических) адресов в таблице ниже 

 | Устройство |         адрес         |  
 |------------|-----------------------|
 |     SW1    |     0003.e419.d701    | 
 |     SW2    |     0040.0b9d.a501    | 
 |     PC-A   |     0002.1755.36E2    | 
 |     PC-B   |     0005.5E64.4C58    |
