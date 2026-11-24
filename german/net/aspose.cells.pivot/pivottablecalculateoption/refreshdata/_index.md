---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableCalculateOption-Eigenschaft. Gibt an, ob die Datenquelle der Pivot-Tabelle aktualisiert wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Gibt an, ob die Datenquelle der PivotTable aktualisiert wird.

```csharp
public bool RefreshData { get; set; }
```

### Hinweise

Wenn sie true ist, wird der Pivot-Cache aus der Datenquelle aktualisiert und anschließend werden alle Pivot-Tabellen basierend auf demselben Pivot-Cache berechnet.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für die Pivot-Tabelle einrichten
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Quellendaten ändern
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Pivot-Tabelle mit der RefreshData-Option berechnen
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Den aktualisierten Pivot-Tabellenwert ausgeben
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### Siehe auch

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


