---
title: "Sınıf WebExtension"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtension sınıfı. Bir Office Eklentisi örneğini temsil eder"
type: docs
url: /tr/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Bir Office Eklentisi örneğini temsil eder.

```csharp
public class WebExtension
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Değiştirilen referansların bir listesini alır. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Bir Office Eklentisi ile belgedeki veri arasındaki tüm bağlama ilişkilerini alır. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Geçerli belgede Office Eklentisi örneğini benzersiz şekilde tanımlayan değeri alır ve ayarlar. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Kullanıcının Office Eklentisiyle etkileşime girip giremeyeceğini gösterir. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Web uzantısının tüm özelliklerini alır. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Bir Office Eklentisine yönelik birincil referansı al. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "YouTube";
            
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 410, 730);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


