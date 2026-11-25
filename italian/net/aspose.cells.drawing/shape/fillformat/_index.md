---
title: "Shape.FillFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce un oggetto MsoFillFormat che contiene le proprietà di formattazione di riempimento per la forma specificata."
type: docs
url: /it/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Restituisce un oggetto MsoFillFormat che contiene le proprietà di formattazione di riempimento per la forma specificata.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà Shape.Fill. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare la proprietà FillFormat.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // Accedi alla proprietà FillFormat (sola lettura).
                MsoFillFormat fillFormat = shape.FillFormat;

                // Visualizza le proprietà attuali di FillFormat.
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // Modifica le proprietà di FillFormat (poiché non è sola lettura).
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Visualizza le proprietà aggiornate di FillFormat.
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Salva la cartella di lavoro
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


