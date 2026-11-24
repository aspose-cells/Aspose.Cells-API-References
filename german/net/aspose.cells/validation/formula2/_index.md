---
title: "Validation.Formula2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist"
type: docs
url: /de/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist.

```csharp
public string Formula2 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // Erstelle Validierung für Zelle B7
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Setze Validierungstyp und Formeln
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Validierung anwenden
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


