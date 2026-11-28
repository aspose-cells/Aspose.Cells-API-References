---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Nesneleri dışa aktarmak için ExportObjectListener'ı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Nesneleri dışa aktarmak için ExportObjectListener'ı alır ve ayarlar.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlSaveOptions.IStreamProvider özelliğini kullanın. Bu özellik, Ağustos 2015'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // Özel bir dışa aktarma nesne dinleyicisi oluşturun
            var listener = new CustomExportObjectListener();
            
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Dinleyici ile HTML kaydetme seçenekleri oluşturun
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // HTML dosyasına kaydedin
            workbook.Save("output.html", saveOptions);
        }
    }

    // IExportObjectListener'ın özel uygulaması
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Örnek: Dışa aktarılan nesneyi işleyin
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Orijinal nesneyi döndürün (gerekirse değiştirilebilir)
            return e;
        }
    }
}
```

### Ayrıca Bakınız

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


