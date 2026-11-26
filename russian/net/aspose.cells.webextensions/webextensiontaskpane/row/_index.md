---
title: "WebExtensionTaskPane.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionTaskPane. Получает и задает индекс, перечисляющий от внешней стороны к внутренней этой панели задач среди других сохраненных панелей, закреплённых в том же расположении по умолчанию"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Получает и задает индекс, перечисляемый от внешнего к внутреннему, этой панели задач среди других сохранённых панелей задач, закреплённых в том же расположении по умолчанию.

```csharp
public int Row { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyRowDemo
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
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Добавить панель задач
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Настроить свойства панели задач
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Продемонстрировать использование свойства Row
            taskPane.Row = 5; // Set row position
            
            // Сохраните книгу
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### См. также

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


