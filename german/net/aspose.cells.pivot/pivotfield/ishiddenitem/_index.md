---
title: "PivotField.IsHiddenItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gibt an, ob das bestimmte PivotItem ausgeblendet ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/ishiddenitem/
---
## PivotField.IsHiddenItem method

Gibt an, ob das bestimmte PivotItem ausgeblendet ist.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItem(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des pivotItem im pivotField. |

### Rückgabewert

Ob das spezifische PivotItem ausgeblendet ist

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsHidden. Diese Methode wird 12 Monate später, seit August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Country";
            worksheet.Cells["A2"].Value = "USA";
            worksheet.Cells["A3"].Value = "Canada";
            worksheet.Cells["A4"].Value = "UK";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Element bei Index 1 (Kanada) ausblenden
            rowField.HideItem(1, true);
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Prüfen, ob das Element bei Index 1 ausgeblendet ist
            bool isHidden = rowField.IsHiddenItem(1);
            Console.WriteLine("Is item at index 1 hidden? " + isHidden);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldIsHiddenItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


