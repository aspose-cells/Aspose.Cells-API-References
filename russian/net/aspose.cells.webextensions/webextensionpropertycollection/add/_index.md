---
title: "WebExtensionPropertyCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WebExtensionPropertyCollection. Добавляет свойство веб-расширения"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

Добавляет свойство веб‑расширения.

```csharp
public int Add(string name, string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| значение | String | Значение свойства. |

### Возвращаемое значение

Индекс добавленного свойства.

### Примеры

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
            
            // Продемонстрировать метод Add с параметрами (String, String)
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


