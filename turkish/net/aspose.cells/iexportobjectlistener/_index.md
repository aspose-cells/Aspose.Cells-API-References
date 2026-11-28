---
title: "Arayüz IExportObjectListener"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IExportObjectListener arayüzü. Kullanıcıların dışa aktarım sırasında nesneleri manipüle etmesine izin verir."
type: docs
url: /tr/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Kullanıcıların dışa aktarım sırasında nesneleri manipüle etmelerine izin verir.

```csharp
public interface IExportObjectListener
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Bir nesneyi dışa aktar. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassIExportObjectListenerDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek bir resim ekleyin
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Özel dışa aktarım dinleyicisi uygulaması
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Özel dinleyici ile HTML olarak kaydet
            workbook.Save("output.html", saveOptions);
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        
        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                if (shape.MsoDrawingType == MsoDrawingType.Picture)
                {
                    string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                    imgIdx++;
                    return url;
                }
            }
            return null;
        }
        
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Gerçek bir uygulamada, burada resmi diske kaydederdiniz
            // Demo amaçları için, sadece sahte bir yol döndürüyoruz
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


