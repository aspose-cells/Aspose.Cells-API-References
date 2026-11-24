---
title: "PivotTable.IsExcel2003Compatible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob die PivotTable bei der Aktualisierung mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, sodass längere Strings abgeschnitten werden. Wenn false, gilt diese Beschränkung nicht. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

Gibt an, ob die PivotTable bei der Aktualisierung mit Excel 2003 kompatibel ist. Ist der Wert true, muss ein String höchstens 255 Zeichen lang sein; überschreitet er diese Länge, wird er abgeschnitten. Ist der Wert false, gilt diese Beschränkung nicht. Der Standardwert ist true.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Ein Arbeitsblatt hinzufügen und mit Beispieldaten füllen
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // Beispiel-Datenzeilen hinzufügen
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // Fügen Sie eine Pivot-Tabelle hinzu
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Konfiguriere PivotTable-Felder
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // Kompatibilitätsmodus setzen
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // Aktualisieren und Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


