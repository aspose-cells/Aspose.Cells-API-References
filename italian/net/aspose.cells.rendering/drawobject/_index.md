---
title: "Classe DrawObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.DrawObject. DrawObject verrà inizializzato e restituito durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

DrawObject verrà inizializzato e restituito durante il rendering.

```csharp
public class DrawObject
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Indica l'oggetto Cell durante il rendering. È possibile accedere a tutte le proprietà della cella. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Indica l'indice della pagina di DrawObject. L'indice della pagina parte da zero. Un foglio contiene diverse pagine durante il rendering. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Indica i byte dell'immagine del grafico o della forma renderizzati durante il rendering. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Indica l'oggetto Shape durante il rendering. È possibile accedere a tutte le proprietà della forma. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Indica l'indice del foglio corrente di DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Indica il numero totale di pagine nel rendering corrente. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Indica il tipo di DrawObject. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // Implementazione personalizzata di DrawObjectEventHandler
    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
    }

    public class DrawObjectDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Aggiungi una forma
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // Crea un'istanza di CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Imposta le opzioni di immagine o di stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Renderizza il foglio in un'immagine
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Salva la cartella di lavoro
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


