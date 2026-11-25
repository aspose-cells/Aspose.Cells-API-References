---
title: "Range.SetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Applica lo stile della cella"
type: docs
url: /it/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Applica lo stile della cella.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | Lo stile della cella. |
| explicitFlag | Booleano | True, sovrascrive solo la formattazione che è impostata esplicitamente. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Imposta lo stile dell'intervallo.

```csharp
public void SetStyle(Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | L'oggetto Style. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // Applica lo stile a una cella
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // Crea un intervallo e applica lo stesso stile
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


