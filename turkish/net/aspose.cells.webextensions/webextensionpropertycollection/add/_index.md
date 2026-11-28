---
title: "WebExtensionPropertyCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionPropertyCollection yöntemi. Web uzantısı özelliği ekler"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Web uzantısı özelliği ekler.

```csharp
public int Add(string name, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| değer | String | Özelliğin değeri. |

### Dönüş Değeri

Eklenen özelliğin dizini.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyCollectionMethodAddWithStringStringDemo
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
            
            // Add yöntemini (String, String) parametreleriyle göster
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


