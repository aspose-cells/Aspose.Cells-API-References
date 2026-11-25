---
title: "StyleFlag.RightBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verranno applicate le impostazioni del bordo destro"
type: docs
url: /it/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Le impostazioni del bordo destro saranno applicate.

```csharp
public bool RightBorder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile con bordi
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Crea un flag di stile e abilita il flag del bordo destro
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Salva la cartella di lavoro
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


