# Amlogic_s905
SRC for Amlogic S905 (Tronsmart Vega S95 Telos Meta Pro) etc.

Для сборки нужного скрипта необходимо наличие утилиты mkimage из пакета u-boot-tools.
Устанавливаем нужный пакет :

sudo apt-get install u-boot-tools

Зайти в нужный каталог, внести изменения в текстовый файл исходного файла и собрать командой :

mkimage -A arm -O linux -T script -C none -d aml_autoscript.txt aml_autoscript

либо 

mkimage -A arm -O linux -T script -C none -d s905_autoscript.txt s905_autoscript

