---
title: "Hyperlink.Area"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Hyperlink. Ottiene l'intervallo del collegamento ipertestuale"
type: docs
url: /it/net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Ottiene l'intervallo dell'hyperlink.

```csharp
public CellArea Area { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Main Menu");
            worksheet.Cells["A3"].PutValue("Chapter 1");
            worksheet.Cells["A4"].PutValue("Chapter 2");
            
            // Aggiungi collegamenti ipertestuali
            int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
            int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");

            // Accedi ai collegamenti ipertestuali e dimostra l'uso della proprietà Area
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            string chapter2Address = "";
            foreach (Hyperlink link in hyperlinks)
            {
                // Verifica se il collegamento ipertestuale è nella cella A4 usando la proprietà Area
                if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
                {
                    chapter2Address = link.Address;
                    break;
                }
            }

            Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


