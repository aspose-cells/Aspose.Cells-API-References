---
title: "PivotField.AddCalculatedItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField‑Methode. Fügt dem Pivot‑Feld ein berechnetes Formelelement hinzu."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

Fügt dem Pivot‑Feld ein berechnetes Formelelement hinzu.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name des Elements. |
| Formel | String | Die Formel des Pivot‑Elements. |

### Hinweise

Unterstützt das Hinzufügen berechneter Elemente nur zu Zeilen‑/Spalten‑Feldern.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodAddCalculatedItemWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "grape";
            sheet.Cells["A3"].Value = "kiwi";
            sheet.Cells["A4"].Value = "grape";
            sheet.Cells["A5"].Value = "kiwi";
            
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 50;
            sheet.Cells["B3"].Value = 70;
            sheet.Cells["B4"].Value = 30;
            sheet.Cells["B5"].Value = 20;

            // Erstelle eine Pivot-Tabelle mit den richtigen Parametern
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Rufen Sie das Pivot‑Feld ab und fügen Sie ein berechnetes Element hinzu.
            PivotField fruitField = pivotTable.RowFields[0];
            fruitField.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldAddCalculatedItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


