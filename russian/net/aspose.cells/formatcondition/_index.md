---
title: FormatCondition
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет условие условного форматирования.
type: docs
weight: 3560
url: /ru/net/aspose.cells/formatcondition/
---
## FormatCondition class

Представляет условие условного форматирования.

```csharp
public class FormatCondition
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Получить экземпляр условного форматирования "AboveAverage". Правило экземпляра по умолчанию выделяет ячейки, которые выше среднего для всех значений в диапазоне. Допустимо только для типа = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Получить экземпляр условного форматирования "ColorScale". Экземпляр по умолчанию - "зелено-желто-красный" 3ColorScale. Допустимо только для type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Получить экземпляр условного форматирования "DataBar". Цвет экземпляра по умолчанию - синий. Допустимо только для типа DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Получает и задает значение или выражение, связанное с условным форматированием. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Получает и задает значение или выражение, связанное с условным форматированием. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Получить экземпляр IconSet условного форматирования. IconSetType экземпляра по умолчанию — TrafficLights31. Допустимо только для type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Получает и задает тип оператора условного формата. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | Приоритет этого правила условного форматирования. Это значение используется для определения того, какой формат должен оцениваться и отображаться. Меньшие числовые значения имеют более высокий приоритет, чем более высокие числовые значения, где '1' — наивысший приоритет. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | True, никакие правила с более низким приоритетом не могут быть применены к этому правилу, когда это правило оценивается как true. Применяется только для Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Получает или устанавливает стиль диапазонов ячеек с условным форматированием. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | Текстовое значение в правиле условного форматирования "текст содержит". Допустимо только для type = containsText, notContainsText, beginWith и EndsWith. Значение по умолчанию равно null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | Применимый период времени в правиле условного форматирования «дата наступления…». Допустимо только для type = timePeriod. Значение по умолчанию — TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Получить экземпляр условного форматирования "Top10". Правило экземпляра по умолчанию выделяет ячейки, чьи значения попадают в верхние 10 скобок. Действительно только для типа Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Получает и устанавливает, является ли тип условного формата. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Получает значение или выражение, связанное с этим условием формата. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Получает формулу условного форматирования ячейки. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Получает значение или выражение условного форматирования ячейки. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Получает значение или выражение, связанное с этим условием формата. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Получает формулу условного форматирования ячейки. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Получает значение или выражение условного форматирования ячейки. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Устанавливает значение или выражение, связанное с этим условием формата. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Устанавливает значение или выражение, связанное с этим условием формата. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Устанавливает значение или выражение, связанное с этим условием формата. |

### Примеры

```csharp

[C#]
  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
  //Добавляет пустое условное форматирование
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
  //Устанавливает диапазон условного формата.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
 
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
 
   //Добавляет условие.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
   //Добавляет условие.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
  //Устанавливает цвет фона.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
  //Сохранение файла Excel
workbook.Save("output.xls");

[VB.NET]

'Создание экземпляра рабочей книги object
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Добавляет пустое условное форматирование
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Устанавливает диапазон условного формата.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
 
'Добавляет условие.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Добавляет условие.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Устанавливает цвет фона.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Сохранение файла Excel
workbook.Save("output.xls")
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
