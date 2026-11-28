---
title: "IExportObjectListener.ExportObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IExportObjectListener yöntemi. Bir nesneyi dışa aktar"
type: docs
url: /tr/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Bir nesneyi dışa aktar.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| e | ExportObjectEvent | Bir nesnenin dışa aktarılması gerektiğinde tetiklenen olay. |

### Dönüş Değeri

Nesnenin dışa aktarım sonucuyla ilgili bilgi. Çalışma kitabını HTML formatına dışa aktarırken nesneleri dışa aktarmak için sonuç, bu dışa aktarılmış nesneyi içeren html dosyasından kaydedilen Görüntüye erişmek için URL dizesidir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // IExportObjectListener'ı uygulayan demo sınıfının bir örneğini oluştur
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // Gerçek bir senaryoda, ExportObjectEvent çerçeve tarafından sağlanır
                // Demo amaçları için, yöntemi null ile çağıracağız
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // Dışa aktarımı işlemek için özel uygulama
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Varsayılan dışa aktarma davranışını kullanmak için değiştirilmiş bir nesneyi veya null'ı döndür
            return null;
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


