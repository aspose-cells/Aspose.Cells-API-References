---
title: "WebExtensionTaskPane.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionTaskPane. Ottiene e imposta l'indice che enumera dall'esterno all'interno di questo riquadro attività tra gli altri riquadri attività persistenti ancorati nella stessa posizione predefinita."
type: docs
url: /it/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Ottiene e imposta l'indice, enumerando dall'esterno all'interno, di questo riquadro tra gli altri riquadri persistenti ancorati nella stessa posizione predefinita.

```csharp
public int Row { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'estensione web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Configura le proprietà dell'estensione web
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Aggiungi un riquadro attività
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Configura le proprietà del riquadro attività
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Dimostra l'uso della proprietà Row
            taskPane.Row = 5; // Set row position
            
            // Salva la cartella di lavoro
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### Vedi anche

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


