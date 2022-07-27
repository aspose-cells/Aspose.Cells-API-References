---
title: Validation
second_title: Aspose.Cells för .NET API-referens
description: Representerar datavalidation.settings.
type: docs
weight: 6200
url: /sv/net/aspose.cells/validation/
---
## Validation class

Representerar datavalidation.settings.

```csharp
public class Validation
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Representerar valideringsvarningsstilen. |
| [Areas](../../aspose.cells/validation/areas) { get; } | Får alla[`CellArea`](../cellarea) som innehåller datavalideringsinställningarna. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Representerar datavalideringsfelmeddelandet. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Representerar titeln på dialogrutan för datavalideringsfel. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Representerar värdet eller uttrycket som är associerat med datavalideringen. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Representerar värdet eller uttrycket som är associerat med datavalideringen. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Indikerar om tomma värden är tillåtna av intervalldatavalideringen. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Indikerar om datavalidering visar en rullgardinslista som innehåller acceptabla värden. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Representerar indatameddelandet för datavalidering. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Representerar titeln på dialogrutan för datavalidering. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Representerar operatören för datavalideringen. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Indikerar om datavalideringsfelmeddelandet kommer att visas när användaren anger ogiltiga data. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Indikerar om inmatningsmeddelandet för datavalidering kommer att visas när användaren väljer en cell i datavalideringsintervallet. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Representerar datavalideringstypen. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Representerar det första värdet som är kopplat till datavalideringen. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Representerar det andra värdet som är associerat med datavalideringen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Tillämpar valideringen på området. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Tillämpar valideringen på området. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Tillämpar valideringen på givna områden. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Kopiavalidering. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Hämtar värdet eller uttrycket som är kopplat till denna validering. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket som är associerat med denna validering för specifik cell. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Hämtar värdet eller uttrycket som är kopplat till denna validering. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket som är associerat med denna validering för specifik cell. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Hämta värdet för lista över valideringen för den angivna cellen. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Ta bort valideringsinställningarna i cellen. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Ta bort valideringsinställningarna i intervallet. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Tar bort denna validering från givna områden. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Anger värdet eller uttrycket som är associerat med denna validering. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Anger värdet eller uttrycket som är associerat med denna validering. |

### Exempel

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

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
