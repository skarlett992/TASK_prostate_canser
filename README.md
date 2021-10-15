# TASK_prostate_canser

Задача заключается в определении стадии рака простаты по цифровой патологии биопсии.
По ссылке https://www.kaggle.com/c/prostate-cancer-grade-assessment доступны материалы:

Два датасета - обучающий и тестовый [train].csv:
Обучающий и тестовый датасеты train.csv изначально расположены в одном файле train.csv. 
Тестовыми данными являются последние 500 строк, тренировочными - остальные более 10000. 
В данном файле доступна информация по наименованию изображения биопсии, оценке по шкале Глисон и стадии рака по ISUP.

train_images:
Цифровая патология (изображения, полученные на биопсии с двух участков опухоли) . Каждое имеет расширение tiff file. 
Целевую переменную имеет только файл train_images.

train_label_masks:
Маски сегментации, показывающие, какие части изображения привели к оценке ISUP. 
Эти маски предназначены для помощи в разработке стратегий выбора наиболее полезных подвыборок изображений.


Необходимо построить модель, предсказывающую по цифровой патологии биопсии стадию рака в соответствии со сканом изображения.

Модель исполнена с помощью передачи обучения из предварительно обученной сети EfficientNetB3 
Реализация доступна по ссылке https://www.kaggle.com/natalyayurina/kernel4a3b468030
____________________________________________________________________________________________________________________________________

The task is to determine the stage of prostate cancer by digital biopsy pathology.
The following materials are available at the link https://www.kaggle.com/c/prostate-cancer-grade-assessment:

Two datasets - training and test [train] .csv:
The train.csv training and test datasets are initially located in the same train.csv file.
Test data are the last 500 lines, training data are the rest more than 10,000.
This file provides information on biopsy image naming, Gleason score and ISUP cancer stage.

train_images:
Digital pathology (images obtained on biopsy from two tumor sites). Each has a tiff file extension.
Only the train_images file has a target variable.

train_label_masks:
Segmentation masks showing which parts of the image led to the ISUP score.
These masks are intended to help you develop strategies for selecting the most useful subsamples of images.


It is necessary to build a model that predicts the stage of cancer in accordance with the scanned image by digital biopsy pathology.

The model is executed using a learning transfer from a pretrained EfficientNetB3 network
The implementation is available at https://www.kaggle.com/natalyayurina/kernel4a3b468030
