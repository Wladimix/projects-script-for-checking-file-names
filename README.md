
<div align="center">
  <img src="https://github.com/devicons/devicon/blob/master/icons/php/php-original.svg" title="PHP" alt="PHP" width="300" height="300">
</div>

## Скрипт для проверки наличия файлов по имени
### Описание скрипта
Скрипт проверяет, существуют ли конкретные файлы в указанных папках. В именах файлов должна присутствовать дата (год и месяц), по которой скрипт определит, за какие месяцы каких файлов не хватает. Корневая директория поиска и директории файлов прописываются в config-файле, как и год с месяцем, с которых должен осуществляться поиск конкретного файла. Работа скрипта опирается на словарь, также прописанный в config-файле. Он переводит нужные месяцы в именах файлов в регулярные выражения. В словаре можно указать, по каким месяцам искать файлы. Либо прописать кварталы. Всё зависит от дат в именах искомых файлов.
### Пример config
```
    'Оплата_Ухтинская_управляющая_компания' => [
        'начальный год' => '2022',
        'начальный месяц' => '05',
        'папка' => 'Жилищные_услуги_и_общедомовое_имущество_ООО_Ухтинская_управляющая_компания',
        'словарь' => [
            '01' => '\.01',
            '02' => '\.02',
            '03' => '\.03',
            '04' => '\.04',
            '05' => '\.05',
            '06' => '\.06',
            '07' => '\.07',
            '08' => '\.08',
            '09' => '\.09',
            '10' => '\.10',
            '11' => '\.11',
            '12' => '\.12',
        ]
    ]
```
