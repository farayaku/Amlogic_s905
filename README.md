# Amlogic S905 S905X S912 \ S805 S802 S812
SRC for Amlogic S905 S905X S912 \ S805 S802 S812.

Скрипты, которые находяться в каталоге S805 , предназначенны для использования на платформах S802 S805 S812.

The scripts are in the directory S805 intended for use on platforms S802 S805 S812.

Для сборки нужного скрипта необходимо наличие утилиты mkimage из пакета u-boot-tools.
Устанавливаем нужный пакет :

To build the desired script, you must have mkimage utility from the package u-boot-tools.
Install the desired package :

sudo apt-get install u-boot-tools

Зайти в нужный каталог, внести изменения в файл s905_autoscript.txt  , сохранить изменения и собрать командой :

Go to desired directory, make changes in the file s905_autoscript.txt, save the changes and run command :

mkimage -A arm -O linux -T script -C none -d aml_autoscript.txt aml_autoscript

или 

either

mkimage -A arm -O linux -T script -C none -d s905_autoscript.txt s905_autoscript


