---
title: "LoadOptions.CheckDataValid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Kontrollera om data är giltiga i mallfilen"
type: docs
url: /sv/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Kontrollera om data är giltiga i mallfilen.

```csharp
public bool CheckDataValid { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ med CheckDataValid satt till false
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // Läs in arbetsbok med dessa alternativ
            Workbook workbook = new Workbook("example.xlsx", options);

            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till viss datavalidering för demonstration
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Ange valideringsområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


