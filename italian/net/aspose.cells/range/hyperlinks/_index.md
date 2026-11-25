---
title: "Range.Hyperlinks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce tutti i collegamenti ipertestuali nell'intervallo"
type: docs
url: /it/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Ottiene tutti i collegamenti ipertestuali nell'intervallo.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un collegamento ipertestuale alla cella A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Crea un intervallo che contiene A1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Ottieni i collegamenti ipertestuali nell'intervallo
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Visualizza le informazioni del collegamento ipertestuale
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Elimina il collegamento ipertestuale
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Verifica che il collegamento ipertestuale sia stato rimosso
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


