---
title: "DrawObject.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DrawObject. Indica il tipo di DrawObject"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/type/
---
## DrawObject.Type property

Indica il tipo di DrawObject.

```csharp
public DrawObjectEnum Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    public class DrawObjectPropertyTypeDemo
    {
        // Gestore personalizzato che legge e visualizza la proprietà Type di ciascun DrawObject
        private class TypeReaderHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}, Page: {drawObject.CurrentPage}/{drawObject.TotalPages}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Popola alcune celle
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Aggiungi una forma per generare anche oggetti di disegno di tipo forma
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Imposta le opzioni di rendering con il nostro gestore di disegno personalizzato
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new TypeReaderHandler()
                };

                // Esegui il rendering del foglio – questo attiva gli eventi DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectTypeDemo.png");

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("DrawObjectTypeDemo.xlsx");
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

* enum [DrawObjectEnum](../../drawobjectenum/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


