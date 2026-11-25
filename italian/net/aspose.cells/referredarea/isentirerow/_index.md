---
title: "ReferredArea.IsEntireRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. Indica se quest'area contiene tutte le colonne (intera riga)"
type: docs
url: /it/net/aspose.cells/referredarea/isentirerow/
---
## ReferredArea.IsEntireRow property

Indica se quest'area contiene tutte le colonne (intera riga).

```csharp
public bool IsEntireRow { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Creare un intervallo denominato che fa riferimento all'intera riga 2
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$2:$2";

            // Ottenere l'area di riferimento dell'intervallo denominato
            ReferredArea referredArea = workbook.Worksheets.Names["NamedRange1"].GetReferredAreas(false)[0];

            // Visualizzare il valore corrente di IsEntireRow
            Console.WriteLine("IsEntireRow value for NamedRange1: " + referredArea.IsEntireRow);

            // Creare un altro intervallo denominato che fa riferimento a un intervallo specifico (non all'intera riga)
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Ottenere l'area di riferimento del secondo intervallo denominato
            ReferredArea referredArea2 = workbook.Worksheets.Names["NamedRange2"].GetReferredAreas(false)[0];

            // Visualizzare il valore corrente di IsEntireRow per il secondo intervallo
            Console.WriteLine("IsEntireRow value for NamedRange2: " + referredArea2.IsEntireRow);

            // Dimostrare l'effetto di IsEntireRow controllando le dimensioni dell'intervallo
            Console.WriteLine("NamedRange1 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("NamedRange2 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Salva la cartella di lavoro
            workbook.Save("ReferredAreaPropertyIsEntireRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


