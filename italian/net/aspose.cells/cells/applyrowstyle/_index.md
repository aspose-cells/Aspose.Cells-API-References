---
title: "Cells.ApplyRowStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Applica formati per un'intera riga"
type: docs
url: /it/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Applica formati a un'intera riga.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| stile | Stile | L'oggetto stile che verrà applicato. |
| flag | StyleFlag | Flag che indicano le proprietà di formattazione applicate. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile con bordi
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Crea un flag di stile per i bordi
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Applica lo stile alla prima riga
            cells.ApplyRowStyle(0, style, styleFlag);

            // Salva la cartella di lavoro
            workbook.Save("ApplyRowStyleDemo.xlsx");
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


