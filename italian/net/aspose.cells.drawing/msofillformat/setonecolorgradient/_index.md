---
title: "MsoFillFormat.SetOneColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo MsoFillFormat. Imposta il riempimento specificato a un gradiente a un colore"
type: docs
url: /it/net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

Imposta il riempimento specificato a un gradiente a un colore.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | Un colore di gradiente. |
| grado | Double | Il grado del gradiente. Può essere un valore da 0.0 (scuro) a 1.0 (chiaro). |
| stile | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 50, 50);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Imposta un gradiente a un colore con parametri specificati
            fillFormat.SetOneColorGradient(Color.Red, 0.5, GradientStyleType.DiagonalUp, 2);

            workbook.Save("GradientFillExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


