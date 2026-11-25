---
title: "StyleFlag.BottomBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Le impostazioni del bordo inferiore saranno applicate"
type: docs
url: /it/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Le impostazioni del bordo inferiore verranno applicate.

```csharp
public bool BottomBorder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea uno stile con le impostazioni del bordo inferiore
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Crea flag di stile e abilita la modifica del bordo inferiore
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Applica lo stile con il flag alla cella A1
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
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


