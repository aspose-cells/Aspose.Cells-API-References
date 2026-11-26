---
title: "WebExtensionTaskPaneCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPaneCollection. Obtiene el panel de tareas por el índice específico"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpanecollection/item/
---
## WebExtensionTaskPaneCollection indexer

Obtiene el panel de tareas por el índice específico.

```csharp
public WebExtensionTaskPane this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

El panel de tareas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPaneCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpane", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            // Demostrar el uso de la propiedad Item
            WebExtensionTaskPane retrievedPane = taskPanes[paneIndex];
            Console.WriteLine($"Retrieved task pane width: {retrievedPane.Width}");

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionTaskPane](../../webextensiontaskpane/)
* class [WebExtensionTaskPaneCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


