---
title: "DrawObject.Cell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DrawObject özelliği. Render sırasında Cell nesnesini gösterir. Hücrenin tüm özelliklerine erişilebilir"
type: docs
url: /tr/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Render ederken Cell nesnesini gösterir. Hücrenin tüm özelliklerine erişilebilir.

```csharp
public Cell Cell { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // DrawObject olaylarını yakalamak ve Cell özelliğini okumak için özel işleyici
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Temel çizim nesnesi bilgilerini çıktılayın
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Salt okunur Cell özelliğini okumayı gösterin
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
                // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Hücrelere bazı örnek veriler ekle
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Şekil çizim olaylarının da tetiklenmesini sağlamak için bir şekil ekleyin
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Özel çizim işleyicimizle render seçeneklerini ayarlayın
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Çalışma sayfasını render edin – bu DrawObject olaylarını tetikleyecek
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Çalışma kitabını kaydedin (isteğe bağlı)
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

### Ayrıca Bakınız

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


