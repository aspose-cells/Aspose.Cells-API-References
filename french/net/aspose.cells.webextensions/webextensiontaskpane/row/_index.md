---
title: "WebExtensionTaskPane.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionTaskPane. Obtient et définit l'index énumérant de l'extérieur vers l'intérieur de ce volet de tâche parmi les autres volets persistants ancrés au même emplacement par défaut"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Obtient et définit l'index, en énumérant de l'extérieur vers l'intérieur, de ce volet de tâche parmi les autres volets de tâche persistants ancrés au même emplacement par défaut.

```csharp
public int Row { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une extension web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Configurer les propriétés de l'extension web
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Ajouter un volet de tâche
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Configurer les propriétés du volet de tâche
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Démontrer l'utilisation de la propriété Row
            taskPane.Row = 5; // Set row position
            
            // Enregistrez le classeur
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### Voir aussi

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


