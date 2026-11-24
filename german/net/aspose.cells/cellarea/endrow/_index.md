---
title: "CellArea.EndRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellArea-Feld. Ruft die Endzeile dieses Bereichs ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Liest oder setzt die Endzeile dieses Bereichs.

```csharp
public int EndRow;
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // PivotTable hinzufügen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Zeilenfeld und Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Demonstrieren Sie die Verwendung von EndRow
            Console.WriteLine("Pivot table ends at row: " + pivotTable.TableRange2.EndRow);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTable_EndRow_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


