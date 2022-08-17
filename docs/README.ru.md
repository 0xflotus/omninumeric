# Omninumeric

![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cu-numbers) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/cu-numbers) [![Codecov](https://img.shields.io/codecov/c/github/endrain/cu-numbers)](https://app.codecov.io/gh/endrain/cu-numbers)

[![PyPI - License](https://img.shields.io/pypi/l/cu-numbers)](./LICENSE.ru) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

🌏 [English](./README.md) Русский

Программа для преобразования чисел между арабской и церковнославянской системами записи.

## Историческая справка

[В этой статье](./INTRODUCTION.ru.md) вы можете ознакомиться с церковнославянской системой записи чисел.

## Установка

	pip install cu-numbers

## Использование

	import cunumbers.cunumbers as cu

	#   Преобразовать арабское число в церковнославянское
	#   Принимает ненулевой int, возвращает str

	a = cu.to_cu(1)
	
	#   Преобразовать церковнославянское число в арабское
	#   Принимает непустой str, возвращает int

	b = cu.to_arab("а҃")

В обоих направлениях поддерживаются варианты записи "сплошной" и "по группам". Запись "по группам" используется по умолчанию для преобразования в ЦСЯ.

Метод `to_cu()` принимает несколько флагов:

	#   CU_PLAIN устанавливает "сплошной" вариант записи для преобразования в ЦСЯ

	c = cu.to_cu(111111, CU_PLAIN)
	
	#   CU_NOTITLO опускает вывод знака "титло"

	d = cu.to_cu(11000, CU_PLAIN | CU_NOTITLO)

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
