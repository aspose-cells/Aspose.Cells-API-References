---
title: "WebExtensionTaskPane.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionTaskPane. Indica se il Task Pane è visibile per impostazione predefinita quando il documento si apre"
type: docs
url: /it/net/aspose.cells.webextensions/webextensiontaskpane/isvisible/
---
## WebExtensionTaskPane.IsVisible property

Indica se il Task Pane è visualizzato come visibile per impostazione predefinita quando il documento si apre.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'estensione web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Configura le proprietà dell'estensione web
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Aggiungi un riquadro attività
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Configura le proprietà del riquadro attività
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.Width = 300;
            
            // Dimostra la proprietà IsVisible
            Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
            taskPane.IsVisible = true;
            Console.WriteLine("After setting to true: " + taskPane.IsVisible);
            
            // Salva la cartella di lavoro
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


