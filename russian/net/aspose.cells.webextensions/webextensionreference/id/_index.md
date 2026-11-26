---
title: "WebExtensionReference.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionReference. Получает и задает идентификатор, связанный с Office Addin в рамках поставщика каталога. Идентификатор ДОЛЖЕН быть уникальным в пределах поставщика каталога."
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Получает и задает идентификатор, связанный с Office Add-in в провайдере каталога. Идентификатор ДОЛЖЕН быть уникальным в пределах провайдера каталога.

```csharp
public string Id { get; set; }
```

### Примеры

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
            
            // Установка свойства Id и других ссылочных свойств
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Добавление свойств веб‑расширения
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Добавление формы и привязка веб‑расширения
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Сохранить и проверить
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


