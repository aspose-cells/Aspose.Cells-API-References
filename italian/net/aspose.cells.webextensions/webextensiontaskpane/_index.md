---
title: "Classe WebExtensionTaskPane"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionTaskPane. Rappresenta un oggetto taskpane persistente"
type: docs
url: /it/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Rappresenta un oggetto taskpane persistente.

```csharp
public class WebExtensionTaskPane
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Ottiene e imposta l'ultima posizione di aggancio di questo oggetto taskpane. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Indica se il taskpane è bloccato al documento nell'interfaccia utente e non può essere chiuso dall'utente. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Indica se il Task Pane è visualizzato come visibile per impostazione predefinita quando il documento si apre. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Ottiene e imposta l'indice, enumerando dall'esterno all'interno, di questo riquadro tra gli altri riquadri persistenti ancorati nella stessa posizione predefinita. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Ottiene e imposta la parte dell'estensione web associata all'istanza del riquadro. |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Ottiene e imposta il valore di larghezza predefinito per questa istanza del riquadro. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


