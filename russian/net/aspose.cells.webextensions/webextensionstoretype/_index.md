---
title: "Перечисление WebExtensionStoreType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.WebExtensions.WebExtensionStoreType. Представляет тип хранилища веб‑расширения"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Представляет тип хранилища веб‑расширения.

```csharp
public enum WebExtensionStoreType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| OMEX | `0` | Указывает, что тип хранилища — Office.com. |
| SPCatalog | `1` | Указывает, что тип хранилища — корпоративный каталог SharePoint. |
| SPApp | `2` | Указывает, что тип хранилища — веб‑приложение SharePoint. |
| Exchange | `3` | Указывает, что тип хранилища — сервер Exchange. |
| FileSystem | `4` | Указывает, что тип хранилища — общая папка файловой системы. |
| Registry | `5` | Указывает, что тип хранилища — системный реестр. |
| ExCatalog | `6` | Указывает, что тип хранилища — централизованное развертывание через Exchange. |

### Примеры

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

### См. также

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


