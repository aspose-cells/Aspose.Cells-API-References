---
title: "DrawObject.TotalPages"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DrawObject. Indica il numero totale di pagine nel rendering corrente"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Indica il numero totale di pagine nel rendering corrente.

```csharp
public int TotalPages { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyTotalPagesDemo
    {
        // Gestore personalizzato per catturare gli eventi DrawObject e leggere la proprietà TotalPages
        private class TotalPagesHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Visualizza il valore della proprietà TotalPages
                Console.WriteLine($"Total Pages in Rendering: {drawObject.TotalPages}");
                Console.WriteLine($"Current Page: {drawObject.CurrentPage + 1}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio per rendere significativo il rendering
                sheet.Cells["A1"].PutValue("Sample Data");
                sheet.Cells["A2"].PutValue("More Data");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Aggiungi una forma per garantire la generazione di più oggetti di disegno
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura le opzioni di rendering con il nostro gestore personalizzato
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = false, // Allow multiple pages to demonstrate TotalPages
                    DrawObjectEventHandler = new TotalPagesHandler()
                };

                // Esegui il rendering del foglio di lavoro - questo attiverà gli eventi DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "TotalPagesDemo.png");

                // Salva la cartella di lavoro
                workbook.Save("TotalPagesDemo.xlsx");
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


