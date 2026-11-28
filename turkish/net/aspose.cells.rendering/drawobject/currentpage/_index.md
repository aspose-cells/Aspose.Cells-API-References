---
title: "DrawObject.CurrentPage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DrawObject özelliği. DrawObject'in sayfa indeksini gösterir. Sayfa indeksi sıfırdan başlar. Bir Sheet render sırasında birden fazla sayfa içerir"
type: docs
url: /tr/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

DrawObject'in sayfa indeksini gösterir. Sayfa indeksi sıfırdan başlar. Bir Sheet render ederken birkaç sayfa içerir.

```csharp
public int CurrentPage { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // CurrentPage özelliğini okuyup görüntülemek için özel işleyici
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // CurrentPage özelliği değerini görüntüleyin
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
                // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Render'ı anlamlı kılmak için bazı örnek veriler ekleyin
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Şekil tipi çizim nesneleri oluşturmak için bir şekil ekleyin
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Özel çizim işleyicimizle render seçeneklerini ayarlayın
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Çalışma sayfasını render edin ve DrawObject olaylarını tetikleyin
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


