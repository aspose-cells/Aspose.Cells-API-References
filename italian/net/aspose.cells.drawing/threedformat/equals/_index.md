---
title: "ThreeDFormat.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ThreeDFormat."
type: docs
url: /it/net/aspose.cells.drawing/threedformat/equals/
---
## ThreeDFormat.Equals method

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per confrontare i formati 3D
            Shape shape1 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 150, 100, 100, 0, 0);

            // Ottieni i formati 3D delle forme
            ThreeDFormat format1 = shape1.ThreeDFormat;
            ThreeDFormat format2 = shape2.ThreeDFormat;

            // Configura impostazioni 3D identiche
            format1.BottomBevelWidth = 10;
            format1.BottomBevelHeight = 10;
            format1.BottomBevelType = BevelType.ArtDeco;

            format2.BottomBevelWidth = 10;
            format2.BottomBevelHeight = 10;
            format2.BottomBevelType = BevelType.ArtDeco;

            try
            {
                // Chiama il metodo Equals per confrontare i formati 3D
                bool areEqual = format1.Equals((object)format2);

                // Visualizza il risultato
                Console.WriteLine($"The 3D formats are equal: {areEqual}");

                // Modifica una proprietà per renderli diversi
                format2.BottomBevelWidth = 15;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, the 3D formats are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ThreeDFormatEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


