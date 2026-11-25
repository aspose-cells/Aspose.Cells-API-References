---
title: "ReferredArea.StartColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. La colonna iniziale dell'area"
type: docs
url: /it/net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

La colonna iniziale dell'area.

```csharp
public int StartColumn { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["C1"].PutValue("Cherry");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);

            // Crea un intervallo denominato che fa riferimento a B1:C2
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!B1:C2";

            // Ottieni l'area di riferimento con recalculate impostato su false
            ReferredArea referredArea = name.GetReferredAreas(false)[0];

            // Dimostrare la proprietà StartColumn
            Console.WriteLine("Start Column: " + referredArea.StartColumn);
            Console.WriteLine("End Column: " + referredArea.EndColumn);

            // Stampare i valori nell'area di riferimento usando StartColumn
            Cells cells = worksheet.Cells;
            for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
            {
                for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
                {
                    Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
                }
            }
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


