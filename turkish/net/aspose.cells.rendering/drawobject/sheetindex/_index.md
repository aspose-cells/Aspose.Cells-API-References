---
title: "DrawObject.SheetIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DrawObject özelliği. DrawObject'in geçerli sayfa indeksini gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

DrawObject'in geçerli sheet indeksini gösterir.

```csharp
public int SheetIndex { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // Her DrawObject'in SheetIndex'ini okuyan ve görüntüleyen özel işleyici
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
                // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // İçerik oluşturmak için bazı hücreleri doldurun
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Şekil çizim nesnelerinin de oluşturulması için bir şekil ekleyin
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Özel işleyicimizle render seçeneklerini ayarlayın
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // Çalışma sayfasını render edin – bu DrawObject olaylarını tetikler
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // Çalışma kitabını kaydedin (isteğe bağlı)
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

### Ayrıca Bakınız

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


