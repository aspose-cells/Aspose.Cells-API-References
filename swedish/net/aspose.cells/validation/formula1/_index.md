---
title: "Validation.Formula1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Representerar värdet eller uttrycket som är associerat med datavalideringen"
type: docs
url: /sv/net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Representerar värdet eller uttrycket som är associerat med data validation.

```csharp
public string Formula1 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula1Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till listvalidering med Formula1 som kommaseparerade värden
            Validation validation1 = worksheet.Validations[worksheet.Validations.Add()];
            validation1.Type = ValidationType.List;
            validation1.AlertStyle = ValidationAlertType.Stop;
            validation1.Formula1 = "A,B,C";
            validation1.AddArea(new CellArea() { StartRow = 0, StartColumn = 0, EndRow = 5, EndColumn = 0 });

            // Lägg till formelvalidering med Formula1 som cellreferens
            Validation validation2 = worksheet.Validations[worksheet.Validations.Add()];
            validation2.Type = ValidationType.Custom;
            validation2.AlertStyle = ValidationAlertType.Stop;
            validation2.Formula1 = "=A5";
            validation2.AddArea(new CellArea() { StartRow = 0, StartColumn = 1, EndRow = 5, EndColumn = 1 });

            // Spara och ladda om för att verifiera beständighet
            string outputPath = "output_validation_formula1.xlsx";
            workbook.Save(outputPath);

            // Ladda om för att verifiera
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            Console.WriteLine("Validation 1 Formula1: " + loadedSheet.Validations[0].Formula1);
            Console.WriteLine("Validation 2 Formula1: " + loadedSheet.Validations[1].Formula1);
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


