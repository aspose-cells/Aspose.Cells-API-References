---
title: "Sınıf ExportObjectEvent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExportObjectEvent sınıfı. Resim gibi bir nesne dışa aktarılırken tetiklenen olay"
type: docs
url: /tr/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

Resim gibi bir nesne dışa aktarıldığında tetiklenen olay.

```csharp
public class ExportObjectEvent
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Dışa aktarılacak nesneyi alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventDemo
    {
        public static void ExportObjectEventExample()
        {
            // IExportObjectListener'ın özel uygulaması
            // HTML dosyasını özel dinleyiciyle kaydet
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;

        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape shape)
            {
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }

        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Burada resmi herhangi bir konuma kaydedin, ardından oluşturulan HTML'nin resmi alabileceği URL'yi (göreceli veya mutlak) döndürün
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


