---
title: "Enum PivotRefreshState"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotRefreshState enum. Der Zustand für das Aktualisieren von PivotTables"
type: docs
url: /de/net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

Der Zustand zum Aktualisieren von PivotTables.

```csharp
public enum PivotRefreshState
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Success | `0` | Erfolgreich aktualisiert |
| UnsupportedExternalDataSource | `1` | Aktualisierung fehlgeschlagen, weil die Datenquelle extern ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotRefreshStateDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit einer Beispiel‑PivotTable
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // PivotRefreshState demonstrieren
            PivotRefreshState refreshState = pivotTable.RefreshData();
            if (refreshState == PivotRefreshState.Success)
            {
                Console.WriteLine("Pivot table refreshed successfully");
            }
            else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
            {
                Console.WriteLine("External data source not supported - calculating data instead");
                pivotTable.CalculateData();
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PivotRefreshStateDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


