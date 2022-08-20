# ЦЕРКОВНОСЛАВЯНСКАЯ СИСТЕМА ЗАПИСИ ЧИСЕЛ

🌏 [English](./INTRODUCTION.md) Русский

## 1. Цифры
В церковнославянской системе записи чисел отдельные буквы используются для записи цифр от 1 до 9 в регистрах от единиц до сотен - т.е. всего 27 цифр. Нуль отсутствует.

ЦСЯ|Арабские|ЦСЯ|Арабские|ЦСЯ|Арабские
---|---|---|---|---|---
а҃|1|і҃|10|р҃|100
в҃|2|к҃|20|с҃|200
г҃|3|л҃|30|т҃|300
д҃|4|м҃|40|у҃|400
є҃|5|н҃|50|ф҃|500
ѕ҃|6|ѯ҃|60|х҃|600
з҃|7|ѻ҃|70|ѱ҃|700
и҃|8|п҃|80|ѿ҃|800
ѳ҃|9|ч҃|90|ц҃|900

## 2. Базовые числа
Число величиной `x < 1000` (базовое) записывается соответствующими цифрами соответствующих разрядов, от старшего разряда к младшему. Исключение составляют числа от 11 до 19, в которых цифры меняются местами.

**Примеры:**
ЦСЯ|Арабские|ЦСЯ|Арабские|ЦСЯ|Арабские
---|---|---|---|---|---
а҃|1|і҃|10|р҃|100
|||||р҃а|101
|||||р҃і|110
|||а҃і|11|ра҃і|111
|||к҃а|21|рк҃а|121

## 3. Числа от тысячи и больше
В числе величиной `x > 999` для обозначения разряда старшего порядка перед цифрой приписывается отметка - знак тысячи `҂`. За каждый знак тысячи перед цифрой ее величина умножается на 1000.

**Примеры:**
ЦСЯ|Арабские
---|---
҂а҃|1 000
҂і҃|10 000
҂р҃|100 000
҂҂а҃|1 000 000

## 4. Варианты записи чисел
В ЦСЯ существует несколько вариантов записи чисел величиной `x > 999`.

## 4.1. "Сплошная" запись
В "сплошной" записи знаками тысяч отмечается каждая цифра в разрядах старшего порядка. Таким образом, умножается только цифра, непосредственно следующая за знаками.

В этом варианте цифры в числах от 11 до 19 меняются местами только "в натуральном" виде, если не отмечены знаками тысяч.

**Примеры:**
ЦСЯ|Арабские
---|---
҂р҂і҂ара҃і|111 111

## 4.2 Запись "по группам"
В записи с разбиением по группам знаками тысяч отмечается каждая группа цифр, составляющая отдельное базовое число в разряде старшего порядка. Таким образом, умножается все базовое число, непосредственно следующее за знаками.

В этом варианте цифры в числах от 11 до 19 меняются местами всегда, в отличие от "сплошного".

**Примеры:**
ЦСЯ|Арабские
---|---
҂раіра҃і|111 111

## 4.3 Запись "с обводом"
В записи с обводом для обозначения разрядов старшего порядка используется специальный набор отметок, которыми обводятся цифры, находящиеся в разрядах от десяти тысяч до миллиардов.

**Примеры:**
ЦСЯ|Арабские
---|---
а&#1160;а&#8413;҂ара҃і|111 111

## 5. Декорирование

## 5.1 Титло
В записи ЦСЯ чисел обязательно используется надстрочный знак "титло" `҃ `&nbsp;. Титло пишется над второй цифрой с конца, если она существует и не отмечена знаками тысяч. В противном случае титло пишется над последней цифрой числа.

В более древних источниках можно обнаружить другие правила записи титла: например, над второй цифрой сначала, или длинное над всем числом. Последний вариант можно воспроизвести с помощью символов Unicode "титло начало", "титло отрезок", "титло конец".

## 5.2 Точки

Иногда в записи ЦСЯ чисел использовались точки. Точка может стоять после числа, а может быть и по точке с обеих сторон. Точка также может использоваться как дополнительный разделитель разрядов при записи "по группам". В некоторых случаях это даже необходимо, чтобы избежать двусмысленности:

||ЦСЯ|Арабские
|---|---|---
|Запись "сплошная":|҂і҂а҃|11000
|Запись "по группам":|҂а҃і|11000
||҂а.і҃|1010