---
title: "WebExtensionReference.StoreName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionReference. Ottiene e imposta l'istanza del marketplace in cui è memorizzato l'Office Add-in."
type: docs
url: /it/net/aspose.cells.webextensions/webextensionreference/storename/
---
## WebExtensionReference.StoreName property

Ottiene e imposta l'istanza del marketplace in cui è archiviato l'Office Add-in.

```csharp
public string StoreName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyStoreNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'estensione web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Imposta le proprietà di riferimento dell'estensione web includendo StoreName
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Aggiungi un riquadro attività per l'estensione web
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            // Salva la cartella di lavoro
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension saved successfully.");
        }
    }
}
```

### Vedi anche

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


