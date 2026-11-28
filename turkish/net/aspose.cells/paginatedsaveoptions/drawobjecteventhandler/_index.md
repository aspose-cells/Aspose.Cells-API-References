---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Render ederken DrawObject ve Bound'ı almak için bu arayüzü uygular"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Renderleme sırasında DrawObject ve Bound elde etmek için bu arabirimi uygular.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı örnek veri ve şekiller ekleyin
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Sayfalı kaydetme seçenekleri örneği oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Özelliğin mevcut değerini gösterin (başlangıçta null olmalı)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Yeni bir özel olay işleyicisi ayarlayın
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Bu, render sırasında Draw yöntemini tetikleyecek
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Farkı göstermek için olay işleyicisini null yapın
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


