---
title: "WebExtensionTaskPane.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionTaskPane. Obtient et définit la valeur de largeur par défaut pour cette instance de volet de tâche"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensiontaskpane/width/
---
## WebExtensionTaskPane.Width property

Obtient et définit la valeur de largeur par défaut pour cette instance de volet de tâche.

```csharp
public double Width { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
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
            
            // Démontrer l’utilisation de la propriété Width
            taskPane.Width = 350;
            
            workbook.Save("WebExtensionTaskPanePropertyWidthDemo.xlsx");
            
            Console.WriteLine("Workbook saved with task pane width set to: " + taskPane.Width);
        }
    }
}
```

### Voir aussi

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


