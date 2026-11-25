---
title: "DrawObject.SheetIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DrawObject. Indica l'indice del foglio corrente di DrawObject"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

Indica l'indice del foglio corrente di DrawObject.

```csharp
public int SheetIndex { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // Gestore personalizzato che legge e visualizza il SheetIndex di ciascun DrawObject
    class SheetIndexReaderHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
            Console.WriteLine($"Page: {drawObject.CurrentPage + 1}/{drawObject.TotalPages}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
            Console.WriteLine();
        }
    }

    public class DrawObjectPropertySheetIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Popola alcune celle per avere contenuto da renderizzare
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Aggiungi una forma affinché gli shape draw objects vengano generati anche
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura le opzioni di rendering con il nostro gestore personalizzato
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // Esegui il rendering del foglio di lavoro – questo attiva gli eventi DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("SheetIndexDemo.xlsx");
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

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


