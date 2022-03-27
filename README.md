# hse_hw3_chromhmm

Выбранная клеточная линия: `HepG2`.

Ссылка на *GoogleColab*: https://colab.research.google.com/drive/1AckR-C3DC6wrR9fcHPOHISEXHj0QIMiH?usp=sharing

## Часть 1

#### Таблица с используемыми гистоновыми метками:

| Название гистоновой метки | Имя файла |
| ------- | ----------- |
| H3k27me3	| H3k27me3StdAlnRep1.bam	|
| H3k36me3 |	H3k36me3StdAlnRep1.bam	|
|	H3k27ac |	H3k27acStdAlnRep1.bam  |
|	H3k79me2 |	H3k79me2StdAlnRep1.bam  |
|	H3k9me3 |	H3k09me3AlnRep1.bam	|
|	H3k4me1 |	H3k04me1StdAlnRep1.bam	|
|	H3k4me2 |	H3k4me2StdAlnRep1.bam	|
|	H2az |	H2azStdAlnRep.bam	|
| H3k4me3 |	H3k4me3StdAlnRep1.bam	|
| H3k9ac |	H3k9acStdAlnRep1.bam	|

#### Полученные изображения из выдачи ChromHMM:

<p float="left">
  <img src="/ChromHMM/emissions_10.png" width="350" />
  <img src="/ChromHMM/transitions_10.png" width="350" />
  <img src="/ChromHMM/Hepg2_10_overlap.png" width="350" />
  <img src="/ChromHMM/Hepg2_10_RefSeqTES_neighborhood.png" width="400" />
  <img src="/ChromHMM/Hepg2_10_RefSeqTSS_neighborhood.png" width="400" />
</p>

#### Таблица c обозначениями эпигенетических типов

| State | Характерные гистоновые метки | Описание | Название эпигенетического типа |
| ----- | ---------------------------- | -------- | ------------------------------ |
|   1   | - | Низкий сигнал | Transcribed weak |
|   2   | H3K7me9 | Низкий сигнал для 1 метки | Transcribed |
|   3   | H3K7me9, H3k4me1  | Относительно сильный сигнал для 2 меток | weak enhancer |
|   4   |  H3k4me1 | Относительно сильный сигнал для 1 гистоновой метки | weak enhancer |
|   5   |  H3k4me2, H3k4me1 | Относительно сильный сигнал | strong enhancer |
|   6   | H3k4me3, H3k4me2, H3k9ac, | Сильный сигнал | Promoter active |
|   7   | H3k4me2, H3k4me1 | Средний сигнал | Promoter weak |
|   8   |	 H3k27me3  | Низкий сигнал | Repressed |
|   9   |  -  | Нет сигнала, самый больщой % генома | Repetitive |
|   10  | H3k9me3 | Чащего всего ассоциирован с laminb1lads | Insulator |


#### Скрины различных участков на примере для типов 1, 2, 9:

| State | Скрин с genome.ucsc                      |
| ----- | ---------------------------------------- |
|   1   | <img src="/img/1.png" width="500" /> |
|   2   | <img src="/img/2.png" width="500" /> |
|   9   |	<img src="/img/9.png" width="500" /> |


## Часть 2 (Бонус)
<img src="/img/bonus.png" width="800" />
