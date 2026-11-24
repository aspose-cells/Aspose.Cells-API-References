---
title: "Range.CurrentRegion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt. Die aktuelle Region ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt wird."
type: docs
url: /de/net/aspose.cells/range/currentregion/
---
## Range.CurrentRegion property

Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt. Die aktuelle Region ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt ist.

```csharp
public Range CurrentRegion { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyCurrentRegionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle Daten mit einigen leeren Zellen, um Regionen zu erzeugen
            worksheet.Cells["A1"].PutValue("Region 1");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Lasse Zeile 5 leer, um Regionen zu trennen
            
            worksheet.Cells["A6"].PutValue("Region 2");
            worksheet.Cells["A7"].PutValue("Data 4");
            worksheet.Cells["B7"].PutValue("Data 5");
            worksheet.Cells["A8"].PutValue("Data 6");

            // Erhalte eine Zelle in der ersten Region und konvertiere sie in einen Range
            Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
            Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
            
            Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
            Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);

            // Erhalte eine Zelle in der zweiten Region und konvertiere sie in einen Range
            Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
            Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
            
            Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
            Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);

            // Wende Formatierung auf die gesamte aktuelle Region an
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            currentRegion1.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


