---
title: "DrawObject.Cell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DrawObject. Indica l'oggetto Cell durante il rendering. È possibile accedere a tutte le proprietà della cella"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Indica l'oggetto Cell durante il rendering. È possibile accedere a tutte le proprietà della cella.

```csharp
public Cell Cell { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // Gestore personalizzato per catturare gli eventi DrawObject e leggere la proprietà Cell
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Genera informazioni di base sul draw object
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Dimostra la lettura della proprietà Cell di sola lettura
            if (drawObject.Cell != null)
            {
                var cell = drawObject.Cell;
                Console.WriteLine($"Cell Name: {cell.Name}");
                Console.WriteLine($"Cell Value: {cell.Value}");
                Console.WriteLine($"Cell Row: {cell.Row}, Column: {cell.Column}");
            }
        }
    }

    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Aggiungi alcuni dati di esempio alle celle
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Aggiungi una forma per garantire che gli shape draw events vengano sollevati anche
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura le opzioni di rendering con il nostro custom draw handler
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Esegui il rendering del foglio di lavoro – questo attiverà gli eventi DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("DrawObjectCellDemo.xlsx");
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


