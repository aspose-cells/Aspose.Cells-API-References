---
title: "UnionRange.RefersTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Ottiene a cosa si riferiscono gli intervalli"
type: docs
url: /it/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Ottiene a cosa si riferisce l'intervallo.

```csharp
public string RefersTo { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Crea un intervallo denominato
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Crea un intervallo di unione che includa il nostro intervallo nominato
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Visualizza la proprietà RefersTo dell'intervallo di unione
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Crea un altro intervallo e visualizza il suo RefersTo
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // Dimostra l'uso di RefersTo per identificare la composizione dell'intervallo
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Mostra come RefersTo cambia quando gli intervalli vengono modificati
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Salva la cartella di lavoro
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


