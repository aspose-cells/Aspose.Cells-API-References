---
title: "FillFormat.SetTwoColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FillFormat. Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | Color | Un colore di gradiente. |
| color2 | Color | Due colori di gradiente. |
| stile | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma semplice per dimostrare il riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // Ottieni il formato di riempimento della forma
            FillFormat fillFormat = shape.Fill;

            // Imposta un gradiente a due colori con i parametri specificati
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // Salva la cartella di lavoro
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | Color | Un colore di gradiente. |
| transparency1 | Double | Il grado di trasparenza del colore1 come valore da 0.0 (opaco) a 1.0 (trasparente). |
| color2 | Color | Due colori di gradiente. |
| transparency2 | Double | Il grado di trasparenza del colore2 come valore da 0.0 (opaco) a 1.0 (trasparente). |
| stile | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma rettangolare per dimostrare la formattazione del riempimento
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // Prepara i parametri per SetTwoColorGradient
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // Chiama SetTwoColorGradient con parametri specifici
                fillFormat.SetTwoColorGradient(
                    color1, 
                    transparency1, 
                    color2, 
                    transparency2, 
                    gradientStyle, 
                    variant
                );

                Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
            }

            // Salva la cartella di lavoro per mostrare l'effetto
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


