---
title: "Enum LightRigDirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Rappresenta il tipo di direzione del rig luminoso"
type: docs
url: /it/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Rappresenta il tipo di direzione del rig di luce.

```csharp
public enum LightRigDirectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Bottom | `0` | Inferiore |
| BottomLeft | `1` | In basso a sinistra. |
| BottomRight | `2` | In basso a destra. |
| Left | `3` | Sinistra. |
| Right | `4` | Destra. |
| Top | `5` | In alto. |
| TopLeft | `6` | In alto a sinistra. |
| TopRight | `7` | In alto a destra. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la direzione del rig luce
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Imposta la direzione del rig luce per il formato 3D della forma
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Dimostra diverse direzioni del rig luce
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Cambia la direzione del rig luce
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Itera attraverso tutte le possibili direzioni del rig luce
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Salva la cartella di lavoro
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


