---
title: "PivotField.IsHiddenItemDetail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gibt an, ob die Details des jeweiligen PivotItem ausgeblendet werden sollen"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Gibt an, ob die Details des jeweiligen PivotItem ausgeblendet werden sollen..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des pivotItem im pivotField. |

### Rückgabewert

ob das Detail des jeweiligen PivotItem ausgeblendet ist

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsDetailHidden. Diese Methode wird 12 Monate später, ab August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // PivotTable hinzufügen
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // PivotField abrufen
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Detail des Elements für Index 1 (USA) ausblenden
            pivotField.HideItemDetail(1, true);
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Prüfen, ob das Detail des Elements ausgeblendet ist
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Arbeitsmappe speichern.
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


