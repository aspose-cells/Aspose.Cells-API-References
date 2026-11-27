---
title: "Worksheet.Validations"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar samlingen av datavalideringsinställningar i arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Hämtar datavalideringsinställningssamlingen i arbetsbladet.

```csharp
public ValidationCollection Validations { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till datavalidering i cell A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Rättelse: Skapa CellArea med StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Hämta validering från cell A1
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Skriv ut valideringstyp
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Spara arbetsboken
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### Se även

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


