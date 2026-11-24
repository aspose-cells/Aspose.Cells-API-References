---
title: "Protection.AllowUsingPivotTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schutz-Eigenschaft. Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt bearbeiten darf"
type: docs
url: /de/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Stellt dar, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblattschutz aktivieren
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Überprüfen Sie die Einstellung
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // Erstelle eine Pivot-Tabelle, um die Funktionalität zu demonstrieren
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Erstelle eine Pivot-Tabelle mit den richtigen Parametern
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


