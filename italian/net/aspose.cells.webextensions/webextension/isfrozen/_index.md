---
title: "WebExtension.IsFrozen"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtension. Indica se l'utente può interagire con l'Office Addin o meno"
type: docs
url: /it/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Indica se l'utente può interagire con l'Office Add-in o meno.

```csharp
public bool IsFrozen { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIsFrozenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Questa riga fallirà perché WebExtension richiede parametri del costruttore
                // WebExtension webExtension = new WebExtension();
                
                // Invece, otterremo un'estensione web dal workbook se possibile
                // oppure dimostrare con un approccio diverso
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // Per scopi dimostrativi, mostreremo come la proprietà funzionerebbe se avessi un'istanza valida
                // In uno scenario reale, otterresti l'istanza WebExtension dal workbook o da un'altra fonte
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // Imposta le proprietà iniziali
                    webExtension.Id = "MyAddin123";
                    
                    // Visualizza il valore iniziale di IsFrozen
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Modifica la proprietà IsFrozen (poiché è leggibile e scrivibile)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Dimostra l'effetto verificando se l'utente può interagire
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Salva il workbook (anche se l'estensione web potrebbe non essere persistita senza passaggi aggiuntivi)
                    workbook.Save("WebExtensionIsFrozenDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static WebExtension GetWebExtensionInstance(Workbook workbook)
        {
            // In una reale implementazione, questo otterrebbe un WebExtension esistente dal workbook
            // oppure crearne uno correttamente con i parametri del costruttore richiesti
            // Questo è solo un segnaposto per la dimostrazione
            return null;
        }
    }
}
```

### Vedi anche

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


