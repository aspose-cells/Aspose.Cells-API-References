---
title: "Style.SetBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Imposta i bordi dello stile"
type: docs
url: /it/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Imposta i bordi dello stile.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderType | BorderType | Il/i bordo/i da impostare, può essere una combinazione di [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | Lo stile del bordo. |
| borderColor | Color | Il colore del bordo. |

### Valore di ritorno

Se le impostazioni attuali del bordo sono state modificate.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            var range = worksheet.Cells.CreateRange("A1:D4");

            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            workbook.Save("BorderExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Imposta i bordi dello stile.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderType | BorderType | Il/i bordo/i da impostare, può essere una combinazione di [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | Lo stile del bordo. |
| borderColor | CellsColor | Il colore del bordo. |

### Valore di ritorno

Se le impostazioni attuali del bordo sono state modificate.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Crea uno stile
                Style style = workbook.CreateStyle();
                
                // Crea un oggetto CellsColor usando il metodo di fabbrica appropriato
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // Chiama SetBorder con i parametri BorderType, CellBorderType e CellsColor
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Applica lo stile a una cella
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Salva la cartella di lavoro
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


