---
title: "WebExtensionTaskPane.IsLocked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionTaskPane. Indica se il riquadro attività è bloccato al documento nell'interfaccia utente e non può essere chiuso dall'utente"
type: docs
url: /it/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

Indica se il taskpane è bloccato al documento nell'interfaccia utente e non può essere chiuso dall'utente.

```csharp
public bool IsLocked { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionTaskPanePropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un riquadro attività tramite la collezione di estensioni web della cartella di lavoro
                WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
                int paneIndex = taskPanes.Add();
                WebExtensionTaskPane taskPane = taskPanes[paneIndex];
                
                Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
                
                taskPane.IsLocked = true;
                Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);

                workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


