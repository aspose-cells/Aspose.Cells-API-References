---
title: "WebExtension.Reference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtension Eigenschaft. Gibt die primäre Referenz zu einem Office Addin zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Liest die primäre Referenz zu einem Office-Add-In.

```csharp
public WebExtensionReference Reference { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Eine Web‑Erweiterung hinzufügen
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Referenz‑Eigenschaften setzen
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Erweiterungs‑Eigenschaften hinzufügen
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
            
            // Task‑Pane hinzufügen
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            // Task‑Pane konfigurieren
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            
            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Web extension with reference properties created successfully.");
        }
    }
}
```

### Siehe auch

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


