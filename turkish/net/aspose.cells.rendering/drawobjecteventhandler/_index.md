---
title: "Class DrawObjectEventHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.DrawObjectEventHandler sınıfı. Render ederken DrawObject ve Bound'ı almak için arabirim"
type: docs
url: /tr/net/aspose.cells.rendering/drawobjecteventhandler/
---
## DrawObjectEventHandler class

Oluşturma sırasında DrawObject ve Bound elde etmek için arayüz.

```csharp
public abstract class DrawObjectEventHandler
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | Renderleme sırasında DrawObject ve Bound elde etmek için bu arabirimi uygular. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(12345);
            worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter

            // Özel render işleyicisi ile PDF kaydetme seçenekleri oluştur
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();

            // Çalışma kitabını PDF'ye render özelleştirmesiyle kaydet
            workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Farklı render nesne türlerinin işlenmesini göster
            switch (drawObject.Type)
            {
                case DrawObjectEnum.Cell:
                    Console.WriteLine($"Rendering cell at ({x}, {y})");
                    break;
                    
                case DrawObjectEnum.Image:
                    Console.WriteLine($"Rendering image at ({x}, {y})");
                    break;
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


