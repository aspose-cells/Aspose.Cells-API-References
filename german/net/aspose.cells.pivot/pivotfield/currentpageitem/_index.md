---
title: "PivotField.CurrentPageItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField‑Eigenschaft. Liest das aktuell angezeigte Seitenelement aus oder legt es fest, nur für dieses PivotField‑Seitenfeld."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Liest oder legt das aktuell angezeigte Seiten-Element für dieses Pivot-Feld fest (nur Seitenfeld).

```csharp
public short CurrentPageItem { get; set; }
```

### Hinweise

Verwenden Sie [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) als Sentinelwert, um „Alle auswählen“ anzuzeigen. Dies ist ein vordefinierter Marker und kein gültiger Elementindex.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Felder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Daten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Seitenfelder abrufen.
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Aktuelle Seitenelemente anzeigen.
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Aktuelles Seitenelement ändern.
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


