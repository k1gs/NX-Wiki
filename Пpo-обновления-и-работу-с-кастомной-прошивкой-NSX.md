# Как обновляться чтобы не получить [бан](https://docs.google.com/document/u/0/d/16hTgzan8DNfzfttIZNMi-4GiUPw_Gn07KxrC8nVbT_g/edit)

Во первых необходимо убедиться что на новую версию прошивки есть весь софт необходимый для вас, чаще всего кефир или чифир.

### **Если у вас кефир**
1. Заходите в **kefir updater**

2. Перейдите в раздел **`Обновить Kefir`**

3. Скачиваете и устанавливаете самую актуальную версию kefir'a

4. После перезагрузки заходим снова в **kefir updater** и переходим в раздел **`Скачать прошивку`**

5. Переходим в **`daybreak`** и выбираем папку firmware 

6. Выбрать из списка драйверов exFat + Fat32

7. После перезагрузки вы имеете свежий кефир + hos

### **Если у вас чифир**

1. Хос вам обновлять не надо чифир 17.0.0 не поддерживает, поэтому обновим сам чифир

2. Заходим в AIO и переходим во вкладку **`Сторонние загрузки`**

3. Спускаемся ниже и нажимаем на **Refresh**

4. После перезапуска AIO возвращаемся и качаем **`4IFIR BETA HOS16.`**

5. После перезагрузки у вас свежий крепкий чифир :)

Порядок обновления: [Эмунанд](https://docs.google.com/document/u/0/d/16hTgzan8DNfzfttIZNMi-4GiUPw_Gn07KxrC8nVbT_g/edit) **->** [Сток через (Semi-stock)](https://docs.google.com/document/u/0/d/16hTgzan8DNfzfttIZNMi-4GiUPw_Gn07KxrC8nVbT_g/edit) чтобы не сжечь [фьюзы](https://docs.google.com/document/u/0/d/16hTgzan8DNfzfttIZNMi-4GiUPw_Gn07KxrC8nVbT_g/edit). 

### Причины по которым в можете попасть в бан

**Так же хочу описать за что вы можете получить бан, некоторые из причин могут дать бан в теории. Но лучше не рисковать**

1. Использование модов в semi-stock

2. Установка пираток в semi-stock (в т.ч homebrew в режиме тайтла и тинфоил)

3. Бан даётся только за откаты прошивки с сожжеными фьюзами

4. Если какое-то действие из вышеперечисленных раннее вы делали в сиснанде то его лучше почистить, иначе бан

5. Разгон в semi-stock

6. Абьюз сохранений из эмунанда в сиснанд

7. Использование читов в онлайн играх





# Обновил прошивку вижу это как быть? Failed to match warm boot with fuses! 

![](https://i.imgur.com/5G3cF9s.png)

Ошибка которая возникает либо при неправильном порядке обновления либо при неправильном способе обновления. У вас сгорели фьюзы.
Может помочь заход в semi-stock, либо в full stock (через more configs -> full stock). Если не сработает то только вариант выше.


**За правки в этом пункте спасибо: metro-2012 и Serj k :)**

# Какие бекапы надо сделать и как? 

**САМЫЕ ВАЖНЫЕ БЭКАПЫ ЭТО ФАЙЛЫ БУТА И ПРОД КЛЮЧИ ИХ ДЕЛАЕМ В 1 ОЧЕРЕДЬ.**

### Бекап boot0 & boot1 файлов

Бекап бут файлов: **hekate -> tools -> backup eMMC -> eMMC BOOT0 & BOOT1**

![](https://i.imgur.com/1BmhAPP.png)

![](https://i.imgur.com/zWCVVHA.png)

*Пример успешного бекапа бутрома*

### Бекап prod.keys

Бекап ключей: **hekate -> payloads -> lockpick rcm -> Dump from sysNAND**

![](https://i.imgur.com/AThEsGh.png)

*Пример успешного бекапа продкючей*

### Бекап RawGPP разделов

Заходите в хикату(при включении консоли нажать **"vol -"**)

Заходим в раздел **tools** -> **backup eMMC** -> **backup RawGPP**

После этого на вашей сд карте начнет создаваться rawnand бекап. Убедитесь что места на сд карте есть: Размер бекапа для лайта, в2, в1 - 32гб. Размера бекапа для оледа - 64гб.

Бекап появится на вашей сд карте в папке **backup** -> **буквы и цифры**

После создания бекапа скиньте его на ваш компьютер или куда удобно. Для того чтобы бекап не весил много, можете сжать его в .zip архив(через winRAR, 7-Zip). Но если у вас на момент бекапа была занята память и прочее, ваш бекап вряд-ли станет очень мало весить. Но его запаковка значительно снизит его размер. 

# Как можно откатить прошивку безопасно если не сжигал фьюзы?

Точно так же как обновляли прошивку качаем через AIO или 
[датабазу оф.прошивок](https://darthsternie.net/switch-firmwares/). После файлы прошивки можно закинуть в корень сд карты (чтобы было удобнее) и создать для них папку с названием “Firmware”. 

После этого в daybreak’e выбираем эту папку. Вам предложит выбрать драйвер сд карты. 

**Выбираем Fat32 + ExFat.**

# Как быть при запуска атмосферы вижу это: A fatal error occurred when running atmosphere

![](https://i.imgur.com/Bg9HxGh.png)

Данная ошибка вызвана повреждением данных атмосферы, либо ваша текущая версия чифира/кефира/сьюта/ультры не поддерживает текущую версию HOS


**В данном случае можно:** 

* Просто переустановить сборку( возможно вы скачали битый файл) либо если ошибка повториться 

* Проделайте все на другой сд карте. Возможно проблема в ней.

# Во время игры не могу через applet mode запустить hbmenu что делать? 

![](https://i.imgur.com/EJEfAkj.png)

Достаточно отключить сис-модуль sys-ftpd. Но это не решение для всех вылеты могут остаться если homebrew которое вы запускаете требует много оперативной памяти.


#  Хочу устанавливать игры через ftp но ловлю эту ошибку как быть? Bind socket to port 5000 failed: address already in use

![](https://i.imgur.com/YkvSNJF.png)


Отключить модул sys-ftpd в тесла-меню: **L+R+UP -> sysmodules -> sys-ftpd.**

# Как можно перейти с чифира на кефир или любую другую сборку? 

Установку рекомендую выполнить начисто но опишу и способ перехода с уже установленной сборкой

### **`Начисто:`**

* Удаляем все папки с флешки **(Кроме Nintendo и EmuMMC, так же папок warmboot_MARIKO, и backup)**

* Закидываем все файлы из архива сборки в корень sd карты

### **`Установка поверх другой сборки(могут начаться проблемы):`**

* Перекинуть все из архива сборки на корень сд карты

* Переместить с заменой если предложит

# Ошибка при запуске: SD card is ExFat

![](https://i.imgur.com/vX45ywW.png)

Переформатируйте карту в Fat32 с размером кластера в 64 кб, используя программу [Rufus](https://github.com/pbatard/rufus/releases)

# Ошибка при запуске: Unknown pkg1 version

![](https://i.imgur.com/MmDDIDl.png)

Обновите вашу сборку, это ошибка говорит о старой версии

# Переход на новом кефире в семи сток и обратно. И заход в OFW

Переход на новом **kefir719**, был осуществлен через оверлей **Uberhand**. 

Для того чтобы открыть его, необходимо нажать комбинацию: **l + R3(правый стик) + Down**.

Для того чтобы перейти в семи-сток нужно, нажать в оверлее стрелку в право, и пролестать в самый низ. После чего нажать на **Semi-stock**, после чего консоль перезагрузится.

Переход обратно осуществлен, по идентичной схеме.

Для захода в OFW достаточно нажать в хикейте **REBOOT -> OFW** либо же установить конфиг на full stock. [Ссылка на скачивание](https://github.com/k1gs/Kefir-Semi-Stock-/releases/download/full/fullstock.ini). Для захода в эмунанд достаточно перезагрузить консоль.

### **Важно**

Если вы перезагрузились в хикейт, вы обнаружите что в хикейте нет семи-стока. А только full-stock + atmosphere. А эмунанд выключен.

Для того чтобы вернуться без всяких проблем и прочего, запуститесь в атмосферу. И войдите в Uberhand и включите Emunand

# Установка линукса на прошитую консоль
**Это перевод статьи с сайта switchroot**

### Подготовка
1. Сд карта размером в 16GB минимум(желательно дополнительная, чтобы ничего не делать с основной), и установленный на ней хикейт(он есть во всех собрках, в т.ч кефир). Компьютер для того чтобы скинуть на него бекапы

2. Скачанный с торрентов l4t(linux for tegra). [Ссылка на скачивание](https://download.switchroot.org/ubuntu/). **Первый файл - прямая ссылка на скачивание через браузер. Второй файл - торрент**

![](https://i.imgur.com/B95C6hN.png)



### Установка
1. Выполните бекапы всех файлов. Для этого зайдите в **tools -> usb tools -> sd card**. И скиньте все папки из карты памяти на компьютер. Если у вас эмунанд на разделе - зайдите в **tools -> backup eMMC -> SD emuMMC Raw Partition** Так же забекапьте boot1/0

2. Заходим в **tools -> partition sd card** и в строке linux выделяем минимум 5gb. 

3. Используя в этом же меню кнопку **sd ums** скидываем содержимое скачанного архива на сд карту

4. Нажмите на кнопку **flash linux** 

5. Возвращаемся в главное меню, и там заходим в **NYX options**

![](https://i.imgur.com/VX6Db45.png)

6. В появившимся меню нажимаем **Dump Joy-Con BT**

7. Возвращайтесь в главное меню и нажмите **More configs** и выбирите там **L4T Ubuntu**. И проводите oobe(первую) настройку ос

8. Можете скинуть ваши бекапы обратно на флешку, если не использовали запасную флешку
### Особенности
В l4t имеется возможность разгона для игры в эмуляторы, и прочего другого. [Ссылка на гайд по разгону](https://wiki.switchroot.org/wiki/linux/linux-features#nvidia-power-profile-applet-nvpmodel)

Имеется полноценная поддержка дока и клаво\мыши

Полностью десктопный репозиторий Ubuntu

