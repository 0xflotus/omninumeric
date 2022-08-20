# Omninumeric

![PyPI - Python Version](https://img.shields.io/pypi/pyversions/omninumeric) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/omninumeric) [![Codecov](https://img.shields.io/codecov/c/github/endrain/omninumeric)](https://app.codecov.io/gh/endrain/omninumeric)

[![PyPI - License](https://img.shields.io/pypi/l/omninumeric)](./LICENSE.ru) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

🌏 [English](./README.md) Русский

Программа для чтения и записи чисел в алфавитных системах записи.

## Поддерживаемые системы записи

- [x] Церковно-славянская
- [] Римская - в работе
- [] Византийская греческая - в работе
- [] Современная греческая - в проекте
- [] Еврейская - в проекте

## Историческая справка

[В этой статье](./INTRODUCTION.ru.md) вы можете ознакомиться с церковнославянской системой записи чисел.

## Установка

	pip install omninumeric

## Использование

	import omninumeric.cyrillic as cu

	#   Преобразовать арабское число в церковнославянское
	#   Принимает ненулевой int, возвращает str

	a = CU.ArabicNumber(1).convert()
	
	#   Преобразовать церковнославянское число в арабское
	#   Принимает непустой str, возвращает int

	b = CU.CyrillicNumber("а҃").convert()

В обоих направлениях поддерживаются варианты записи "сплошной" и "по группам", "сплошная" запись используется по умолчанию.

При записи в ЦСЯ возможно использование слеедующих флагов:

	#   CU_DELIM устанавливает "сплошной" вариант записи в ЦСЯ

	c = cu.to_alphabetic(111111, CU_DELIM)
	
	#   CU_NOTITLO опускает вывод знака "титло"

	d = cu.to_alphabetic(11000, CU_DELIM | CU_NOTITLO)

	#   Следующие флаги управляют декорированием точками:
	#
	#   CU_ENDDOT - выводит точку в конце
	#   CU_WRAPDOT - выводит точки с обеих сторон
	#   CU_DELIMDOT - выводит точки-разделители разрядов. Устанавливает вариант записи "по группам"
	#   CU_ALLDOT - комбинация флагов CU_WRAPDOT и CU_DELIMDOT


## Принять участие

Откройте новую проблему, опишите в ней исправляемый баг или предлагаемый функционал. Затем откройте запрос на слияние, в описании дайте ссылку на проблему.

## Отзывы

Пишите по адресу: amshoor@gmail.com

## История версий

Смотрите [здесь](./CHANGELOG.ru.md).
