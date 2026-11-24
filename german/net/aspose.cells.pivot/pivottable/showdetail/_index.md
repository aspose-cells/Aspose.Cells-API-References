---
title: "PivotTable.ShowDetail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Zeigt die Details eines Elements im Datenbereich in einer neuen Tabelle an"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Zeige die Details eines Elements im Datenbereich in einer neuen Tabelle an.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Versatz zur ersten Datenzeile im Datenbereich. |
| columnOffset | Int32 | Versatz zur ersten Datenspalte im Datenbereich. |
| newSheet | Boolean | Zeigt die Details in einem neuen Arbeitsblatt an. |
| destRow | Int32 | Die Zielzeile. |
| destColumn | Int32 | Die Zielspalte. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Details für eine bestimmte Zelle anzeigen
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


