---
title: "PivotTable.ShowReportFilterPageByName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Zeigt alle Berichtsfilterseiten gemäß dem Namen des PivotFields an, das PivotField muss sich in den PageFields befinden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

Zeige alle Berichtfilterseiten basierend auf dem Namen des PivotField an, wobei das PivotField in den PageFields liegen muss.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | String | Der Name des PivotField |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            
            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilen- und Datenfelder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Seitenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
            pivotTable.PageFields[0].Name = "FruitFilter";
            
            // Pivot-Tabelle aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Berichtsfilterseiten nach Namen anzeigen
            pivotTable.ShowReportFilterPageByName("FruitFilter");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


