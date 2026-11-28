---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Emf metafilesi oluşturma ayarı"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Emf metafilesinin render edilmesi için ayar.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Açıklamalar

"EMF+ Dual" olarak tanımlanan EMF metafilesi, hem EMF+ kayıtlarını hem de EMF kayıtlarını içerebilir. Görüntüyü oluşturmak için her iki kayıt türü de, yalnızca EMF+ kayıtları veya yalnızca EMF kayıtları kullanılabilir. EmfPlusPrefer ayarlandığında, sayfaya render edilirken EMF+ kayıtları ayrıştırılır, aksi takdirde yalnızca EMF kayıtları ayrıştırılır. Varsayılan değer EmfOnly'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // EMF gösterimi için resim oluştur
            worksheet.Pictures.Add(10, 10, "example.png");

            // PdfSaveOptions kullanarak EMF ayarlarıyla kaydetme seçeneklerini yapılandır
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Çalışma kitabını EMF ayarlarıyla kaydet
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### Ayrıca Bakınız

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


