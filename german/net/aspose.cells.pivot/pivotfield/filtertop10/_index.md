---
title: "PivotField.FilterTop10"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Filtert nach Werten des Daten-Pivotfelds."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Filtert nach Werten des Daten-Pivotfelds.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| valueFieldIndex | Int32 | Der Index des Datenfelds im Datenbereich. |
| Typ | PivotFilterType | Der Typ der Filterdaten. Kann nur Count, Sum und Percent sein. |
| isTop | Boolean | Gibt an, ob der Filter von oben oder unten kommt |
| itemCount | Int32 | Die Anzahl der Elemente |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            worksheet.Cells["A7"].Value = "Banana";
            worksheet.Cells["A8"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 40;
            worksheet.Cells["B6"].Value = 50;
            worksheet.Cells["B7"].Value = 60;
            worksheet.Cells["B8"].Value = 70;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Top-10-Filter anwenden
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableFilterTop10.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


