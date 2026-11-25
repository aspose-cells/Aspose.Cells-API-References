---
title: "StyleFlag.TopBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verranno applicate le impostazioni del bordo superiore"
type: docs
url: /it/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Le impostazioni del bordo superiore saranno applicate.

```csharp
public bool TopBorder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea uno stile con le impostazioni del bordo superiore
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Crea un flag di stile e abilita la modifica del bordo superiore
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Applica lo stile alla cella A1 con solo il flag del bordo superiore abilitato
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(style, styleFlag);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


