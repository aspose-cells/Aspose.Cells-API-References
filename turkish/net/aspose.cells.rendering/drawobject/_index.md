---
title: "DrawObject sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.DrawObject sınıfı. Render ederken DrawObject başlatılacak ve döndürülecek"
type: docs
url: /tr/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

Oluşturma sırasında DrawObject başlatılacak ve döndürülecektir.

```csharp
public class DrawObject
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Render ederken Cell nesnesini gösterir. Hücrenin tüm özelliklerine erişilebilir. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | DrawObject'in sayfa indeksini gösterir. Sayfa indeksi sıfırdan başlar. Bir Sheet render ederken birkaç sayfa içerir. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Render edilen Chart, Shape'in görüntü baytlarını gösterir. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Render ederken Shape nesnesini gösterir. Shape'in tüm özelliklerine erişilebilir. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | DrawObject'in geçerli sheet indeksini gösterir. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Geçerli render işleminin toplam sayfalarını gösterir. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | DrawObject'in tipini gösterir. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // DrawObjectEventHandler'ın özel uygulaması
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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Bir shape ekle
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // CustomDrawObjectEventHandler örneği oluştur
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Görüntü veya yazdırma seçeneklerini ayarla
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Sheet'i bir görüntüye render et
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Çalışma kitabını kaydedin
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


