---
title: "Style.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta il nome dello style"
type: docs
url: /it/net/aspose.cells/style/name/
---
## Style.Name property

Ottiene o imposta il nome dello stile.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea e applica il primo style denominato
            Style style1 = workbook.CreateStyle();
            style1.Number = 7;
            style1.Name = "Sales";
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Sales Data");
            
            // Crea e applica il secondo style denominato
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 14;
            style2.Font.IsBold = true;
            style2.Font.IsItalic = true;
            style2.Font.Color = System.Drawing.Color.Yellow;
            style2.ForegroundColor = System.Drawing.Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            style2.Name = "Header";
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Header Text");
            
            // Salva la cartella di lavoro
            workbook.Save("StylePropertyNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


