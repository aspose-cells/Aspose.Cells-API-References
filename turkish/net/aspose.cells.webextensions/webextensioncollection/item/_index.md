---
title: "WebExtensionCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionCollection özelliği. Belirli bir indeksle web uzantısını alır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Web uzantısını belirli bir dizine göre alır.

```csharp
public WebExtension this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Web uzantısı.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Web uzantıları koleksiyonunu alın
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Bir web video oynatıcı uzantısı ekleyin
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Web uzantısını tutacak bir şekil ekleyin
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Web uzantısını şekle atayın
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Çalışma kitabını kaydedin
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


