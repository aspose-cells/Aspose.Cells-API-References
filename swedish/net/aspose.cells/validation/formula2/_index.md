---
title: "Validation.Formula2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Representerar värdet eller uttrycket som är associerat med datavalideringen"
type: docs
url: /sv/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Representerar värdet eller uttrycket som är associerat med data validation.

```csharp
public string Formula2 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // Skapa validering för cell B7
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Ange valideringstyp och formler
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Tillämpa validering
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Spara arbetsboken
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


