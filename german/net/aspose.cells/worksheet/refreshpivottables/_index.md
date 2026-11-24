---
title: "Worksheet.RefreshPivotTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Aktualisiert alle PivotTables in diesem Worksheet"
type: docs
url: /de/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Aktualisiert alle PivotTables in diesem Arbeitsblatt.

```csharp
public void RefreshPivotTables()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe aus einer Quell-Excel-Datei, die PivotTables enthält
            Workbook workbook = new Workbook("example.xlsx");
            
            // Hole das erste Arbeitsblatt, das PivotTables enthält
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Alle Pivot-Tabellen im Arbeitsblatt aktualisieren
            worksheet.RefreshPivotTables();
            
            // Die aktualisierte Arbeitsmappe speichern
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Aktualisiert alle PivotTables in diesem Arbeitsblatt.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Option | PivotTableRefreshOption | Die Option zum Aktualisieren der Datenquelle der Pivot-Tabelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // Quellendaten ändern
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // Aktualisierungsoptionen erstellen
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // Ergebnis speichern
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


