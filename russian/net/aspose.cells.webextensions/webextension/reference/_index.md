---
title: "WebExtension.Reference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtension. Получить основную ссылку на надстройку Office"
type: docs
url: /ru/net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Получить основную ссылку на Office Add-in.

```csharp
public WebExtensionReference Reference { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyReferenceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить веб‑расширение
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Установить свойства ссылки
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Добавить свойства расширения
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
            
            // Добавить панель задач
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            // Настроить панель задач
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            
            // Сохраните книгу
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Web extension with reference properties created successfully.");
        }
    }
}
```

### См. также

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


