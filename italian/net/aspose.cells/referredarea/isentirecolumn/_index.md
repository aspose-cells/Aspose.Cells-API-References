---
title: "ReferredArea.IsEntireColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. Indica se quest'area contiene l'intera colonna"
type: docs
url: /it/net/aspose.cells/referredarea/isentirecolumn/
---
## ReferredArea.IsEntireColumn property

Indica se quest'area contiene tutte le righe (intera colonna).

```csharp
public bool IsEntireColumn { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Crea un intervallo denominato che fa riferimento all'intera colonna B
            int index = workbook.Worksheets.Names.Add("PriceColumn");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!$B:$B";

            // Ottenere l'area di riferimento dell'intervallo denominato
            ReferredArea referredArea = workbook.Worksheets.Names["PriceColumn"].GetReferredAreas(false)[0];

            // Visualizza il valore della proprietà IsEntireColumn
            Console.WriteLine("IsEntireColumn value for PriceColumn: " + referredArea.IsEntireColumn);

            // Crea un altro intervallo denominato che fa riferimento a un intervallo specifico (non all'intera colonna)
            int index2 = workbook.Worksheets.Names.Add("ProductRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Ottenere l'area di riferimento del secondo intervallo denominato
            ReferredArea referredArea2 = workbook.Worksheets.Names["ProductRange"].GetReferredAreas(false)[0];

            // Visualizza il valore della proprietà IsEntireColumn per il secondo intervallo
            Console.WriteLine("IsEntireColumn value for ProductRange: " + referredArea2.IsEntireColumn);

            // Dimostra l'effetto di IsEntireColumn controllando le dimensioni dell'intervallo
            Console.WriteLine("PriceColumn dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("ProductRange dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Salva la cartella di lavoro
            workbook.Save("ReferredAreaPropertyIsEntireColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


