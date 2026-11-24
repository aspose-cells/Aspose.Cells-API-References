---
title: "UnionRange.RefersTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt die Bereiche zurück, auf die verwiesen wird"
type: docs
url: /de/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Liefert das 'refers to' des Bereichs.

```csharp
public string RefersTo { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Benannten Bereich erstellen
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Erstelle einen UnionRange, der unseren benannten Bereich einschließt
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Zeige die RefersTo-Eigenschaft des UnionRange an
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Erstelle einen weiteren Bereich und zeige dessen RefersTo an
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // Demonstriere die Verwendung von RefersTo zur Identifizierung der Bereichszusammensetzung
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Zeige, wie sich RefersTo ändert, wenn Bereiche geändert werden
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


