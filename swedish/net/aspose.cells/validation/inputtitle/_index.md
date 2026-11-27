---
title: "Validation.InputTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Validation-egenskap. Representerar titeln på datavalideringens inmatningsdialogruta"
type: docs
url: /sv/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Representerar titeln på dialogrutan för data-validation inmatning.

```csharp
public string InputTitle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett valideringsobjekt
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Ange valideringsområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Ställ in valideringsegenskaper
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Ange egenskaper för inmatningsmeddelandet
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Spara arbetsboken
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // Verifiera InputTitle-egenskapen
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### Se även

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


