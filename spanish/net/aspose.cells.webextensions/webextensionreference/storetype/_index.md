---
title: "WebExtensionReference.StoreType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionReference. Obtiene y establece el tipo de mercado que identifica el atributo store"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionreference/storetype/
---
## WebExtensionReference.StoreType property

Obtiene y establece el tipo de marketplace que identifica el atributo de almacén.

```csharp
public WebExtensionStoreType StoreType { get; set; }
```

### Ejemplos

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

### Ver también

* enum [WebExtensionStoreType](../../webextensionstoretype/)
* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


