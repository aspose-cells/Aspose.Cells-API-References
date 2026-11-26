---
title: "WebExtensionCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionCollection. Возвращает веб-расширение по указанному индексу"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Получает веб‑расширение по конкретному индексу.

```csharp
public WebExtension this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Веб-расширение.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите коллекцию веб-расширений
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Добавьте расширение веб-видеоплеера
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Добавьте фигуру для размещения веб-расширения
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Назначьте веб-расширение фигуре
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Сохраните книгу
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


