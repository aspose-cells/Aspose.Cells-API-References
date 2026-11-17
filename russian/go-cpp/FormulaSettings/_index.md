---
title: "Класс FormulaSettings"
linktitle: "FormulaSettings"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс FormulaSettings. Инкапсулирует объект, представляющий formulasettings в Go."
type: docs
weight: 200
url: /ru/go-cpp/formulasettings/
---

## FormulaSettings class

Настройки формул и вычислений.

```go

type FormulaSettings struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetCalculateOnOpen](./getcalculateonopen/) | Указывает, требуется ли приложению выполнять полное вычисление при открытии книги. |
| [SetCalculateOnOpen](./setcalculateonopen/) | Указывает, требуется ли приложению выполнять полное вычисление при открытии книги. |
| [GetCalculateOnSave](./getcalculateonsave/) | Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений. |
| [SetCalculateOnSave](./setcalculateonsave/) | Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений. |
| [GetForceFullCalculation](./getforcefullcalculation/) | Указывает, вычисляет ли он все формулы каждый раз при запуске вычисления. |
| [SetForceFullCalculation](./setforcefullcalculation/) | Указывает, вычисляет ли он все формулы каждый раз при запуске вычисления. |
| [GetCalculationMode](./getcalculationmode/) | Получает или задает режим расчёта книги в MS Excel. |
| [SetCalculationMode](./setcalculationmode/) | Получает или задает режим расчёта книги в MS Excel. |
| [GetCalculationId](./getcalculationid/) | Указывает версию движка расчётов, используемого для вычисления значений в книге. |
| [SetCalculationId](./setcalculationid/) | Указывает версию движка расчётов, используемого для вычисления значений в книге. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | Указывает, следует ли включать итеративный расчёт для разрешения циклических ссылок. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | Указывает, следует ли включать итеративный расчёт для разрешения циклических ссылок. |
| [GetMaxIteration](./getmaxiteration/) | Максимальное количество итераций для разрешения циклической ссылки. |
| [SetMaxIteration](./setmaxiteration/) | Максимальное количество итераций для разрешения циклической ссылки. |
| [GetMaxChange](./getmaxchange/) | Максимальное изменение для разрешения циклической ссылки. |
| [SetMaxChange](./setmaxchange/) | Максимальное изменение для разрешения циклической ссылки. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Указывает, следует ли устанавливать точность вычисленного результата в соответствии с отображаемыми значениями при расчёте формул. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Указывает, следует ли устанавливать точность вычисленного результата в соответствии с отображаемыми значениями при расчёте формул. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | Указывает, следует ли включать цепочку расчётов для формул. По умолчанию — false. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | Указывает, следует ли включать цепочку расчётов для формул. По умолчанию — false. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Указывает, следует ли сохранять пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Указывает, следует ли сохранять пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |
