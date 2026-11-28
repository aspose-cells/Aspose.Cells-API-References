---
title: "WebExtensionReference.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionReference özelliği. Katalog sağlayıcısı içinde Office Addin ile ilişkili tanımlayıcıyı alır ve ayarlar. Tanımlayıcı, katalog sağlayıcısı içinde benzersiz OLMAK zorundadır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Bir katalog sağlayıcısı içinde Office Eklentisi ile ilişkili tanımlayıcıyı alır ve ayarlar. Tanımlayıcı, bir katalog sağlayıcısı içinde benzersiz OLMALIdır.

```csharp
public string Id { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            // Id özelliğini ve diğer referans özelliklerini ayarlama
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Web uzantısı özellikleri ekleme
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Şekil ekleme ve web uzantısını bağlama
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Kaydet ve doğrula
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


