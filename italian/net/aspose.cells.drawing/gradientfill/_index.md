---
title: "Classe GradientFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.GradientFill. Rappresenta il riempimento a gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Rappresenta il riempimento sfumato.

```csharp
public class GradientFill : Fill
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | L'angolo del riempimento lineare. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Ottiene il tipo di direzione del gradiente. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Ottiene il tipo di riempimento a gradiente. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Rappresenta la raccolta di punti di arresto del gradiente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Ereditato da [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Ottiene il codice hash.(Ereditato da [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Imposta il tipo di riempimento a gradiente e la direzione. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a un colore. Valido solo per Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Imposta il riempimento a gradiente predefinito del tema. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Imposta il tipo di riempimento su gradiente per accedere alle proprietà del riempimento a gradiente
            shape.Fill.FillType = FillType.Gradient;

            // Ottieni l'istanza di riempimento a gradiente esistente dalla forma
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Configura il gradiente con due colori utilizzando l'istanza esistente
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Salva la cartella di lavoro
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


