---
title: "PivotTable.TableRange2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht einschließlich Seitenfelder enthält. Nur lesbar"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, einschließlich Seitenfelder. Nur lesbar.

```csharp
public CellArea TableRange2 { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange2Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Daten berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Holen Sie sich das TableRange2, das die gesamte Pivot‑Tabelle umfasst
            CellArea tableRange2 = pivotTable.TableRange2;
            Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
                $"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");

            // Erstellen Sie einen Bereich basierend auf TableRange2
            Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
                tableRange2.StartRow, 
                tableRange2.StartColumn, 
                tableRange2.EndRow - tableRange2.StartRow + 1, 
                tableRange2.EndColumn - tableRange2.StartColumn + 1);

            // Geben Sie die Bereichsadresse aus
            Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


