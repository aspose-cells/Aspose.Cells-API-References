---
title: "PivotTable.Fields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Gibt die spezifischen Felder nach Feldtyp zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Ruft die spezifischen Felder nach dem Feldtyp ab.

```csharp
[Obsolete("Use PivotField.GetFields(PivotFieldType) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | PivotFieldType | der Feldtyp. |

### Rückgabewert

die spezifische Feldsammlung

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.GetFields(PivotFieldType). Diese Methode wird 12 Monate später, seit Mai 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "Sheet";

            // Beispieldaten
            ws.Cells[0, 0].PutValue("X");
            ws.Cells[0, 1].PutValue("Y");
            ws.Cells[0, 2].PutValue("Data");

            ws.Cells[1, 0].PutValue("A");
            ws.Cells[1, 1].PutValue("C");
            ws.Cells[1, 2].PutValue(10);

            ws.Cells[2, 0].PutValue("A");
            ws.Cells[2, 1].PutValue("D");
            ws.Cells[2, 2].PutValue(25);

            ws.Cells[3, 0].PutValue("B");
            ws.Cells[3, 1].PutValue("C");
            ws.Cells[3, 2].PutValue(30);

            ws.Cells[4, 0].PutValue("B");
            ws.Cells[4, 1].PutValue("D");
            ws.Cells[4, 2].PutValue(45);

            // Pivot-Tabelle erstellen
            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add("=Sheet!A1:C5", "A7", "PivotTable1");
            PivotTable pt = ptc[index];

            // Felder hinzufügen und die Fields‑Methode mit PivotFieldType demonstrieren
            int fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
            PivotField rowField = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
            PivotField colField = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            PivotField dataField = pt.Fields(PivotFieldType.Data)[fp];

            // Zweites Datenfeld mit prozentualer Berechnung hinzufügen
            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            dataField = pt.Fields(PivotFieldType.Data)[fp];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
            pt.RefreshData();
            pt.CalculateData();

            wb.Save("PivotTableFieldsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


