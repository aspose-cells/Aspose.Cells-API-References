---
title: "Klass Validation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Validation class. Representerar data validation.settings"
type: docs
url: /sv/net/aspose.cells/validation/
---
## Validation class

Representerar data validation.settings.

```csharp
public class Validation
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Representerar valideringsvarningsstilen. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Hämtar alla [`CellArea`](../cellarea/) som innehåller data validation settings. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Representerar felmeddelandet för data validation. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Representerar titeln på dialogrutan för data-validation fel. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Representerar värdet eller uttrycket som är associerat med data validation. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Representerar värdet eller uttrycket som är associerat med data validation. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Indikerar om tomma värden är tillåtna av data validation för intervallet. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Indikerar om data validation visar en rullgardinslista som innehåller godkända värden. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Representerar inmatningsmeddelandet för data validation. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Representerar titeln på dialogrutan för data-validation inmatning. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Representerar operatorn för data validation. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Indikerar om felmeddelandet för data validation kommer att visas när användaren anger ogiltig data. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Indikerar om inmatningsmeddelandet för data validation kommer att visas när användaren markerar en cell i data validation-intervallet. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Representerar typen av data validation. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Representerar det första värdet som är associerat med data validation. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Representerar det andra värdet som är associerat med data validation. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Tillämpar valideringen på området. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Tillämpar valideringen på området. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Tillämpar valideringen på angivna områden. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Kopiera validering. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Hämtar värdet eller uttrycket som är associerat med denna validering. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket som är associerat med denna validering för en specifik cell. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Hämtar värdet eller uttrycket som är associerat med denna validering. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket som är associerat med denna validering för en specifik cell. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Hämta värdet för listan av valideringen för den angivna cellen. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Hämta värdet av valideringen på den specifika cellen. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Ta bort valideringsinställningarna i cellen. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Ta bort valideringsinställningarna i området. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Tar bort denna validering från angivna områden. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Ställer in värdet eller uttrycket som är associerat med denna validering. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Ställer in värdet eller uttrycket som är associerat med denna validering. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definiera ett cellområde för valideringen
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Åtkomst till valideringssamlingen
            ValidationCollection validations = worksheet.Validations;

            // Lägg till en ny validering i samlingen
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Ställ in valideringsegenskaper
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // Spara arbetsboken
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


