---
title: "GradientFill.SetGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GradientFill. Imposta il tipo e la direzione del riempimento gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Imposta il tipo di riempimento a gradiente e la direzione.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | GradientFillType | Tipo di riempimento gradiente. |
| angle | Double | L'angolo. Valido solo per GradientFillType.Linear. |
| direction | GradientDirectionType | Il tipo di direzione. Valido solo per GradientFillType.Radial e GradientFillType.Rectangle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma per applicare il riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Ottieni il gradiente di riempimento della forma
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Chiama SetGradient con parametri specifici: riempimento lineare, 90 gradi, direzione FromCenter
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro per dimostrare l'effetto
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


