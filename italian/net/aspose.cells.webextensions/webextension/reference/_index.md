---
title: "WebExtension.Reference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtension. Ottiene il riferimento principale a un componente aggiuntivo Office"
type: docs
url: /it/net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Ottieni il riferimento primario a un Office Add-in.

```csharp
public WebExtensionReference Reference { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'estensione web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Imposta le proprietà di riferimento
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Aggiungi proprietà dell'estensione
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
            
            // Aggiungi riquadro attività
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            // Configura riquadro attività
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            
            // Salva la cartella di lavoro
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Web extension with reference properties created successfully.");
        }
    }
}
```

### Vedi anche

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


