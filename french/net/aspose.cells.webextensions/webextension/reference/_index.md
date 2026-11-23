---
title: "WebExtension.Reference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtension. Obtient la référence principale à un module complémentaire Office"
type: docs
url: /fr/net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Obtenez la référence principale d'un Office Add-in.

```csharp
public WebExtensionReference Reference { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyReferenceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une extension web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Définissez les propriétés de référence
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Ajoutez des propriétés d'extension
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
            
            // Ajoutez un volet de tâche
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            // Configurez le volet de tâche
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            
            // Enregistrez le classeur
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Web extension with reference properties created successfully.");
        }
    }
}
```

### Voir aussi

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


