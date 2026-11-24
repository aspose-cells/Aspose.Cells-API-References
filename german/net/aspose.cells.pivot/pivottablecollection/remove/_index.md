---
title: "PivotTableCollection.Remove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableCollection-Methode. Löscht die angegebene PivotTable und löscht die PivotTable-Daten"
type: docs
url: /de/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Löscht die angegebene PivotTable und löscht die PivotTable-Daten

```csharp
public void Remove(PivotTable pivotTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable-Objekt |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Abrufen der Pivot-Tabellensammlung
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // Prüfen, ob Pivot-Tabellen vorhanden sind
            if (pivotTables.Count > 0)
            {
                // Erste Pivot-Tabelle abrufen
                PivotTable pivotTable = pivotTables[0];
                
                // Entfernen Sie die Pivot-Tabelle
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableRemoved.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

Löscht die angegebene PivotTable

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable-Objekt |
| keepData | Boolean | Ob die PivotTable-Daten beibehalten werden sollen |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrieren Sie die Remove-Methode mit PivotTable und booleschen Parametern
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // Entfernen Sie die Pivot-Tabelle, aber behalten Sie die Daten (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // Fügen Sie eine weitere Pivot-Tabelle hinzu
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // Entfernen Sie die Pivot-Tabelle und löschen Sie die Daten (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


