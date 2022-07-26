---
title: Validation
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет данные validation.settings.
type: docs
weight: 6200
url: /ru/net/aspose.cells/validation/
---
## Validation class

Представляет данные validation.settings.

```csharp
public class Validation
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Представляет стиль оповещения о проверке. |
| [Areas](../../aspose.cells/validation/areas) { get; } | получает все[`CellArea`](../cellarea) которые содержат настройки проверки данных. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Представляет сообщение об ошибке проверки данных. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Представляет заголовок диалогового окна ошибки проверки данных. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Представляет значение или выражение, связанное с проверкой данных. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Представляет значение или выражение, связанное с проверкой данных. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Указывает, разрешены ли пустые значения при проверке данных диапазона. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Указывает, отображает ли проверка данных раскрывающийся список, содержащий допустимые значения. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Представляет входное сообщение проверки данных. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Представляет заголовок диалогового окна ввода данных для проверки данных. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Представляет оператора для проверки данных. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Указывает, будет ли отображаться сообщение об ошибке проверки данных всякий раз, когда пользователь вводит недопустимые данные. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Указывает, будет ли отображаться входное сообщение проверки данных всякий раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Представляет тип проверки данных. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Представляет первое значение, связанное с проверкой данных. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Представляет второе значение, связанное с проверкой данных. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Применяет проверку к области. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Применяет проверку к области. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Применяет проверку к заданным областям. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Подтверждение копирования. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Получает значение или выражение, связанное с этой проверкой. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Получает значение или выражение, связанное с этой проверкой. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Получить значение списка проверки для указанной ячейки. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Удалить настройки проверки в ячейке. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Удалить настройки проверки в диапазоне. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Удаляет эту проверку из заданных областей. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Задает значение или выражение, связанное с этой проверкой. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Задает значение или выражение, связанное с этой проверкой. |

### Примеры

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.WholeNumber
validation.Operator = OperatorType.Between
validation.Formula1 = "3"
validation.Formula2 = "1234"
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
