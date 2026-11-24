---
title: "WebExtensionReference.StoreName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionReference-Eigenschaft. Gibt die Instanz des Marktplatzes zurück und legt sie fest, in dem das Office-Add-In gespeichert ist."
type: docs
url: /de/net/aspose.cells.webextensions/webextensionreference/storename/
---
## WebExtensionReference.StoreName property

Liest und schreibt die Instanz des Marktplatzes, in dem das Office-Add-in gespeichert ist.

```csharp
public string StoreName { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Eine Web‑Erweiterung hinzufügen
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Festlegen von WebExtension-Referenzeigenschaften einschließlich StoreName
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Ein Taskbereich für die WebExtension hinzufügen
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension saved successfully.");
        }
    }
}
```

### Siehe auch

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


