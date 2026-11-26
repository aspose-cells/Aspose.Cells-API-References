---
title: "WebExtensionTaskPane.IsVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionTaskPane. Указывает, отображается ли панель задач по умолчанию при открытии документа"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensiontaskpane/isvisible/
---
## WebExtensionTaskPane.IsVisible property

Указывает, отображается ли панель задач по умолчанию при открытии документа.

```csharp
public bool IsVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить веб‑расширение
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Настроить свойства веб‑расширения
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Добавить панель задач
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Настроить свойства панели задач
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.Width = 300;
            
            // Продемонстрировать свойство IsVisible
            Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
            taskPane.IsVisible = true;
            Console.WriteLine("After setting to true: " + taskPane.IsVisible);
            
            // Сохраните книгу
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


