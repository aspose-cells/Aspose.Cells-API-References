---
title: "StyleFlag.HorizontalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione di allineamento orizzontale"
type: docs
url: /it/net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

L'impostazione di allineamento orizzontale sarà applicata.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio nelle celle
            worksheet.Cells["A1"].PutValue("Left Aligned");
            worksheet.Cells["B1"].PutValue("Center Aligned");
            worksheet.Cells["C1"].PutValue("Right Aligned");
            
            // Crea stili con diversi allineamenti orizzontali
            Style styleLeft = workbook.CreateStyle();
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            
            Style styleCenter = workbook.CreateStyle();
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            
            Style styleRight = workbook.CreateStyle();
            styleRight.HorizontalAlignment = TextAlignmentType.Right;
            
            // Crea flag di stile per applicare solo l'allineamento orizzontale
            StyleFlag flag = new StyleFlag();
            flag.HorizontalAlignment = true;
            
            // Applica gli stili agli intervalli
            Aspose.Cells.Range rangeLeft = worksheet.Cells.CreateRange("A1:A1");
            rangeLeft.ApplyStyle(styleLeft, flag);
            
            Aspose.Cells.Range rangeCenter = worksheet.Cells.CreateRange("B1:B1");
            rangeCenter.ApplyStyle(styleCenter, flag);
            
            Aspose.Cells.Range rangeRight = worksheet.Cells.CreateRange("C1:C1");
            rangeRight.ApplyStyle(styleRight, flag);
            
            // Salva la cartella di lavoro
            workbook.Save("HorizontalAlignmentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


