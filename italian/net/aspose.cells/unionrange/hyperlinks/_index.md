---
title: "UnionRange.Hyperlinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Restituisce tutti i collegamenti ipertestuali nell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Ottiene tutti i collegamenti ipertestuali nell'intervallo.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni collegamenti ipertestuali alle celle
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Crea un intervallo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Ottieni i collegamenti ipertestuali nell'intervallo
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Visualizza le informazioni su ciascun collegamento ipertestuale
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Salva la cartella di lavoro
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


