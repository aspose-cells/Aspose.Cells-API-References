---
title: "Cells.ApplyColumnStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Applica formattazioni per un'intera colonna"
type: docs
url: /it/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Applica formati a un'intera colonna.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | L'indice della colonna. |
| stile | Stile | L'oggetto stile che verrà applicato. |
| flag | StyleFlag | Flag che indicano le proprietà di formattazione applicate. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Crea uno stile con bordi
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Crea un flag di stile per applicare solo i bordi
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Applica lo stile alla colonna 1 (indice 0)
            cells.ApplyColumnStyle(0, style, sflag);

            // Salva la cartella di lavoro
            workbook.Save("ApplyColumnStyleOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


