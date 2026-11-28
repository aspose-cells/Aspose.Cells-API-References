---
title: "Enum WebExtensionStoreType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtensionStoreType enum. Web uzantısının mağaza tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Web uzantısının depolama türünün temsilidir.

```csharp
public enum WebExtensionStoreType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| OMEX | `0` | Mağaza tipinin Office.com olduğunu belirtir. |
| SPCatalog | `1` | Mağaza tipinin SharePoint kurumsal kataloğu olduğunu belirtir. |
| SPApp | `2` | Mağaza tipinin bir SharePoint web uygulaması olduğunu belirtir. |
| Exchange | `3` | Depolama türünün bir Exchange sunucusu olduğunu belirtir. |
| FileSystem | `4` | Depolama türünün bir dosya sistemi paylaşımı olduğunu belirtir. |
| Registry | `5` | Depolama türünün sistem kayıt defteri olduğunu belirtir. |
| ExCatalog | `6` | Depolama türünün Exchange aracılığıyla Merkezi Dağıtım olduğunu belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionStoreTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            webExt.Properties.Add("sku", "\"peoplebar-giant\"");
            webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
            webExt.Properties.Add("shape", "\"muscle-people\"");
            webExt.Properties.Add("layout-element-title", "\"NUMBERS ABOUT THE APP\"");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            workbook.Save("WebExtensionStoreTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


