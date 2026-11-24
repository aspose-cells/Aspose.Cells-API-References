---
title: "Cell.GetValidation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt die auf diese Zelle angewendete Validierung zurück."
type: docs
url: /de/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Liefert die auf diese Zelle angewendete Validierung.

```csharp
public Validation GetValidation()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf Zelle B5 zu und fügen Sie eine Validierung hinzu.
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Setzen Sie den Validierungstyp und zeigen Sie eine Nachricht an.
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationDemo.xlsx");
            
            // Überprüfen Sie die Validierung.
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### Siehe auch

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


