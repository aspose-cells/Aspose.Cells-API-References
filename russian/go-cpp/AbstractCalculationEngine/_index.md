---
title: "Класс AbstractCalculationEngine"
linktitle: "AbstractCalculationEngine"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс AbstractCalculationEngine. Инкапсулирует объект, представляющий abstractcalculationengine в Go."
type: docs
weight: 200
url: /ru/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | Пропускает вычисление всей формулы, которая ссылается на функцию, находящуюся в текущей оценке. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | Указывает, требуется ли этому движку буквальный текст параметра во время вычисления.Значение по умолчанию — false. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | Указывает, требуется ли этому движку вычислять параметр в режиме массива. Значение по умолчанию — false.Если CalculationData.GetParamValueInArrayMode(int, int, int) требуется при вычислении customfunctions и пользователь не обновил их определение (через Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), это свойство должно быть установлено в true. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Определяет, должны ли встроенные функции, поддерживаемые встроенным движком, проверяться и обрабатываться этой реализацией.По умолчанию — false. |
| [ForceRecalculate](./forcerecalculate/) | Определяет, следует ли принудительно всегда пересчитывать данную функцию при вычислении общих формул. |
