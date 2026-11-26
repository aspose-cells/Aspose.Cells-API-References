---
title: "Класс WebExtension"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.WebExtensions.WebExtension class. Представляет экземпляр Office Addin."
type: docs
url: /ru/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Представляет экземпляр Office Add-in.

```csharp
public class WebExtension
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Получает список альтернативных ссылок. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Получает все отношения привязок между Office Add-in и данными в документе. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Получает и задает уникальный идентификатор экземпляра Office Add-in в текущем документе. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Указывает, может ли пользователь взаимодействовать с Office Add-in или нет. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Получает все свойства веб-расширения. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Получить основную ссылку на Office Add-in. |

### Примеры

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

### См. также

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


