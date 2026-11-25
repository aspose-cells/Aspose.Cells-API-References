---
title: "Workbook.CountOfStylesInPool"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene il numero degli stili nel pool di stili"
type: docs
url: /it/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Ottiene il numero degli stili nel pool di stili.

```csharp
public int CountOfStylesInPool { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Ottieni il conteggio iniziale degli stili nel pool
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Aggiungi alcuni stili modificando le celle
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Stile 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Stile 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Ottieni il conteggio aggiornato degli stili
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Salva per dimostrare la persistenza degli stili
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


