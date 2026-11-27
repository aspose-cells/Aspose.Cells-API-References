---
title: "Validation.InCellDropDown"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Anger om datavalidering visar en rullgardinslista som innehåller godkända värden"
type: docs
url: /sv/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Indikerar om data validation visar en rullgardinslista som innehåller godkända värden.

```csharp
public bool InCellDropDown { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en validering för cell A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Ställ in valideringstyp till lista med värden
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Aktivera in‑cell‑dropdown
            validation.InCellDropDown = true;

            // Skapa ytterligare en validering för cell B1 utan rullgardin
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Spara arbetsboken
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


