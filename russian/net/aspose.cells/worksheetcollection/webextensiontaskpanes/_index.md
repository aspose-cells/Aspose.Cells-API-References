---
title: "WorksheetCollection.WebExtensionTaskPanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Получает список панелей задач"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/webextensiontaskpanes/
---
## WorksheetCollection.WebExtensionTaskPanes property

Получает список панелей задач.

```csharp
public WebExtensionTaskPaneCollection WebExtensionTaskPanes { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyWebExtensionTaskPanesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить веб‑расширение
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Настроить свойства веб‑расширения
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Добавить и настроить панель задач
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            // Сохраните книгу
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension task pane created successfully.");
        }
    }
}
```

### См. также

* class [WebExtensionTaskPaneCollection](../../../aspose.cells.webextensions/webextensiontaskpanecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


