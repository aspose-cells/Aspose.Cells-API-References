---
title: "GradientFill.SetTwoColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GradientFill. Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/settwocolorgradient/
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per applicare il riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Imposta il tipo di riempimento a gradiente
                shape.Fill.FillType = FillType.Gradient;

                // Ottieni il riempimento gradiente
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Chiama SetTwoColorGradient con parametri realistici
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    Color.Blue,         // color2
                    GradientStyleType.DiagonalDown,  // style
                    1);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, Blue, DiagonalDown, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Salva la cartella di lavoro per dimostrare l'effetto
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
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

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradient297116Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per applicare il riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Imposta il tipo di riempimento a gradiente
                shape.Fill.FillType = FillType.Gradient;

                // Ottieni il riempimento gradiente
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Chiama SetTwoColorGradient con parametri realistici
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    0.5,                // transparency1 (50% transparent)
                    Color.Blue,         // color2
                    0.3,                // transparency2 (30% transparent)
                    GradientStyleType.Horizontal,  // style
                    2);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, 0.5, Blue, 0.3, Horizontal, 2)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Salva la cartella di lavoro per dimostrare l'effetto
            workbook.Save("SetTwoColorGradientWithTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


