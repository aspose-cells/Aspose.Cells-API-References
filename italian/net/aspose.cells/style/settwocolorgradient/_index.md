---
title: "Style.SetTwoColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Imposta il riempimento specificato a un gradiente a due colori"
type: docs
url: /it/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Imposta il riempimento specificato a un gradiente a due colori.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | Color | Un colore di gradiente. |
| color2 | Color | Due colori di gradiente. |
| gradientStyleType | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un oggetto stile
            Style style = workbook.CreateStyle();

            // Imposta un gradiente a due colori per lo style
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Verifica le impostazioni del gradiente
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Salva la cartella di lavoro
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


