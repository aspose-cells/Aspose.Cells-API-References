---
title: "ExportObjectEvent.GetSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportObjectEvent yöntemi. Dışa aktarılacak nesneyi alır"
type: docs
url: /tr/net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Dışa aktarılacak nesneyi alır.

```csharp
public object GetSource()
```

### Dönüş Değeri

dışa aktarılacak nesne.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // GetSource işlevselliğini göstermek için bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Özel bir dışa aktarma nesne dinleyicisi oluşturun
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // ExportObjectEvent'i tetiklemek için çalışma kitabını kaydet
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // GetSource yöntemini göster
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


