---
title: "Classe WebExtensionTaskPane"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionTaskPane. Représente un objet de volet de tâche persistant"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Représente un objet de volet de tâche persistant.

```csharp
public class WebExtensionTaskPane
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Obtient et définit le dernier emplacement ancré de cet objet de volet de tâche. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Indique si le volet de tâche est verrouillé au document dans l’interface utilisateur et ne peut pas être fermé par l’utilisateur. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Indique si le volet de tâche est affiché visible par défaut lorsque le document s’ouvre. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Obtient et définit l'index, en énumérant de l'extérieur vers l'intérieur, de ce volet de tâche parmi les autres volets de tâche persistants ancrés au même emplacement par défaut. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Obtient et définit la partie d'extension web associée à l'instance du volet de tâche |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Obtient et définit la valeur de largeur par défaut pour cette instance de volet de tâche. |

### Exemples

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

### Voir aussi

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


