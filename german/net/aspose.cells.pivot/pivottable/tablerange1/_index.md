---
title: "PivotTable.TableRange1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable property. Gibt ein CellArea‑Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable‑Bericht enthält, jedoch keine Seitenfelder. Nur lesbar"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/tablerange1/
---
## PivotTable.TableRange1 property

Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, jedoch keine Seitenfelder einschließt. Nur lesbar.

```csharp
public CellArea TableRange1 { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange1Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein Arbeitsblatt mit Beispieldaten hinzu
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Erstelle eine Pivot-Tabelle
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            int pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            
            // Felder zur Pivot-Tabelle hinzufügen
            int labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // PivotTable konfigurieren
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // TableRange1‑Eigenschaft demonstrieren
            Console.WriteLine("Pivot Table Range:");
            Console.WriteLine($"Start Row: {pivotTable.TableRange1.StartRow}");
            Console.WriteLine($"End Row: {pivotTable.TableRange1.EndRow}");
            Console.WriteLine($"Start Column: {pivotTable.TableRange1.StartColumn}");
            Console.WriteLine($"End Column: {pivotTable.TableRange1.EndColumn}");

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePropertyTableRange1Demo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


