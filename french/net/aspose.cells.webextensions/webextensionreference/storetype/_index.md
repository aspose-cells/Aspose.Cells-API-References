---
title: "WebExtensionReference.StoreType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionReference. Obtient et définit le type de marché que l'attribut store identifie"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionreference/storetype/
---
## WebExtensionReference.StoreType property

Obtient et définit le type de marketplace que l’attribut de magasin identifie.

```csharp
public WebExtensionStoreType StoreType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyStoreTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\server\path\to\addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            workbook.Save("WebExtensionStoreTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [WebExtensionStoreType](../../webextensionstoretype/)
* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


