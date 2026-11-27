---
title: "Validation.InputMessage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Representerar datavalideringens inmatningsmeddelande"
type: docs
url: /sv/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Representerar inmatningsmeddelandet för data validation.

```csharp
public string InputMessage { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa validering
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Ange egenskaper för inmatningsmeddelandet
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Spara arbetsboken
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


