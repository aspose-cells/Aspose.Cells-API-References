---
title: "Worksheet.Validations"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Sammlung der Datenvalidierungseinstellungen im Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab.

```csharp
public ValidationCollection Validations { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datenvalidierung zu Zelle A1 hinzufügen
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Fix: CellArea mit StartRow, StartColumn, EndRow, EndColumn erstellen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Validierung von Zelle A1 abrufen
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Validierungstyp ausgeben
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


