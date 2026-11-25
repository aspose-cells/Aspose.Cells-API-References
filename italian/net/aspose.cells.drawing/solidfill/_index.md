---
title: "Classe SolidFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.SolidFill. Incapsula l'oggetto che rappresenta il formato di riempimento solido"
type: docs
url: /it/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Incapsula l'oggetto che rappresenta il formato di riempimento solido

```csharp
public class SolidFill : Fill
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Ottiene e imposta l'oggetto [`CellsColor`](./cellscolor/). |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Ottiene o imposta il colore. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Ottiene il codice hash. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una semplice forma rettangolare al foglio
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Configura la forma per utilizzare un riempimento solido
                rect.Fill.FillType = FillType.Solid;

                // Ottieni l'oggetto SolidFill
                SolidFill solidFill = rect.Fill.SolidFill;

                // Imposta le proprietà del riempimento solido
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Accedi alla proprietà CellsColor (lettura/scrittura)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Salva la cartella di lavoro per verificare l'aspetto della forma
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


