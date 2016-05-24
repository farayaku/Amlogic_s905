# Amlogic_s905
SRC for Amlogic S905 (Tronsmart Vega S95 Telos Meta Pro) etc.

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


