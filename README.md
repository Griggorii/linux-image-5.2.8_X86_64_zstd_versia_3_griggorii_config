# linux-image-5.2.8_X86_64_zstd_versia_3_griggorii_config
linux kernel deb X86_64 zstd ubuntu minimum size

Внимание в этом конфиге нет поддержки udf для dvd дисков вышло новое ядро тут эта поддержка добавлена https://github.com/Griggorii/linux-image-5.2.8_X86_64_zstd_versia_4_griggorii_config

Griggorii@gmail.com

Сконфигурировал конфиг что бы ядро в деб формате весило не более 40 мегабайт и работало всё только что мне нужно , работа 
была сложная в семь этапов то блютус не работал то юсб модем и подключаемые устройства , но в конце удалось заставить всё 
это работать и исключить лишний код который возможно придуман зря если всё будет работать и на этом ядре с малым весом.
Скачать уже готовые deb https://drive.google.com/open?id=1fjw2Mwge2iUxm4Ds_LvGa8BF4nQKZ5nT 

В этом конфиге 7 тысяч с лишним строк против 10 тысяч тут https://github.com/Griggorii/linux-image-5.2.8_X86_64_zstd_versia_2_griggorii_config/blob/master/Griggorii_versia_2.config


Переименовываем Griggorii_.config в папке kernel в .config и из терминала 
выполняем

make -j4 bindeb-pkg

-j4 это у меня столько ядер у вас может быть меньше или больше если больше 
то ещё быстрее закончится компиляция.
