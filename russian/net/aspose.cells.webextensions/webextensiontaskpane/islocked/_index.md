---
title: "WebExtensionTaskPane.IsLocked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionTaskPane. Указывает, заблокирована ли панель задач к документу в пользовательском интерфейсе и не может ли пользователь её закрыть"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

Указывает, заблокирована ли панель задач к документу в пользовательском интерфейсе и не может ли пользователь её закрыть.

```csharp
public bool IsLocked { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionTaskPanePropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать панель задач через коллекцию веб‑расширений книги
                WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
                int paneIndex = taskPanes.Add();
                WebExtensionTaskPane taskPane = taskPanes[paneIndex];
                
                Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
                
                taskPane.IsLocked = true;
                Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);

                workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


