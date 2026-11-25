---
title: "Font.Size"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta la dimensione del carattere"
type: docs
url: /it/net/aspose.cells/font/size/
---
## Font.Size property

Ottiene o imposta la dimensione del carattere.

```csharp
public int Size { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il testo con diverse dimensioni di carattere
            Cell cell1 = worksheet.Cells["A1"];
            cell1.Value = "Text with size 12";
            Style style1 = workbook.CreateStyle();
            style1.Font.Size = 12;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A3"];
            cell2.Value = "Text with size 16";
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 16;
            cell2.SetStyle(style2);

            // Salva la cartella di lavoro
            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


