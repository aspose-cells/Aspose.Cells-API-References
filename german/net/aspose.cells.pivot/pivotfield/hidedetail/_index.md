---
title: "PivotField.HideDetail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Legt fest, ob die Details aller PivotItems in einem Pivot-Feld ausgeblendet werden. Das bedeutet, dieses Feld ein- bzw. ausklappen."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Legt fest, ob die Details aller PivotItems in einem Pivot-Feld ausgeblendet werden. Das bedeutet, dieses Feld ein- bzw. ausklappen.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isHiddenDetail | Boolean | Ob die Details des Pivot-Feldes ausgeblendet werden sollen. |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen bitte PivotItemsCollection.HideAllDetails() und UnhideAllDetails() Methode. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Details für das erste Zeilenfeld ausblenden
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


