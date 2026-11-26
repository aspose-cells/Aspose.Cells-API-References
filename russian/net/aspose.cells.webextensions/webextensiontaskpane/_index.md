---
title: "Класс WebExtensionTaskPane"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WebExtensions.WebExtensionTaskPane. Представляет сохранённый объект панели задач"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Представляет сохранённый объект области задач.

```csharp
public class WebExtensionTaskPane
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Получает и задает последнее закреплённое расположение этого объекта панели задач. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Указывает, заблокирована ли панель задач к документу в пользовательском интерфейсе и не может ли пользователь её закрыть. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Указывает, отображается ли панель задач по умолчанию при открытии документа. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Получает и задает индекс, перечисляемый от внешнего к внутреннему, этой панели задач среди других сохранённых панелей задач, закреплённых в том же расположении по умолчанию. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Получает и задает часть веб‑расширения, связанную с экземпляром панели задач |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Получает и задает значение ширины по умолчанию для этого экземпляра панели задач. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionTaskPaneDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


