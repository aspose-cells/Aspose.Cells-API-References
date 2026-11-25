---
title: "DrawObject.CurrentPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DrawObject. Indica l'indice di pagina di DrawObject. L'indice di pagina parte da zero. Un Sheet contiene diverse pagine durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Indica l'indice della pagina di DrawObject. L'indice della pagina parte da zero. Un foglio contiene diverse pagine durante il rendering.

```csharp
public int CurrentPage { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // Gestore personalizzato per leggere e visualizzare la proprietà CurrentPage
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Visualizza il valore della proprietà CurrentPage
                Console.WriteLine($"CurrentPage: {drawObject.CurrentPage}");
                Console.WriteLine($"TotalPages: {drawObject.TotalPages}");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi alcuni dati di esempio per rendere significativo il rendering
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Aggiungi una forma per generare shape-type draw objects
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura le opzioni di rendering con il nostro custom draw handler
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Esegui il rendering del foglio di lavoro per attivare gli eventi DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Salva la cartella di lavoro
                workbook.Save("CurrentPageDemo.xlsx");
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


