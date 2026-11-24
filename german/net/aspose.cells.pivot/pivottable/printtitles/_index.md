---
title: "PivotTable.PrintTitles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt sind. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/printtitles/
---
## PivotTable.PrintTitles property

Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt werden. Der Standardwert ist false.

```csharp
public bool PrintTitles { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintTitlesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt und einige Beispieldaten hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Konfiguriere PivotTable-Felder
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demonstriere die PrintTitles-Eigenschaft
            pivotTable.PrintTitles = true;
            Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePrintTitlesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


