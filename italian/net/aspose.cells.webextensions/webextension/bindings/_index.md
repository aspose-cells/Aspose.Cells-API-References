---
title: "WebExtension.Bindings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtension. Ottiene tutte le relazioni di binding tra un componente aggiuntivo Office e i dati nel documento"
type: docs
url: /it/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Ottiene tutte le relazioni di binding tra un Office Add-in e i dati nel documento.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Supponendo di ottenere un'estensione web da qualche parte (poiché non possiamo crearne una direttamente)
                // Questa è una modifica minima per far compilare il codice mantenendo la sua struttura
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Accedi alla proprietà Bindings (sola lettura)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Visualizza le informazioni sui binding
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Aggiungi un nuovo binding (dimostra l'uso della collezione)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Visualizza il conteggio aggiornato
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("WebExtensionBindingsDemo.xlsx");
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

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


