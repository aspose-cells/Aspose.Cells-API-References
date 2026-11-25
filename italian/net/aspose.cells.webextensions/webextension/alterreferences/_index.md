---
title: "WebExtension.AlterReferences"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtension. Ottiene un elenco di riferimenti alternativi"
type: docs
url: /it/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Ottiene un elenco di alter references.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Ottieni la collezione di estensioni web dal workbook
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Aggiungi una nuova web extension
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Accedi alla proprietà AlterReferences (sola lettura)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Visualizza le informazioni sui riferimenti alter
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Aggiungi un nuovo riferimento alter (dimostra l'uso della collezione)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Visualizza il conteggio aggiornato
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Salva la cartella di lavoro
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


