---
title: "WebExtension.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtension. Ottiene e imposta l'identificatore unico dell'istanza del componente aggiuntivo Office nel documento corrente"
type: docs
url: /it/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Ottiene e imposta l'identificatore univoco dell'istanza di Office Add-in nel documento corrente.

```csharp
public string Id { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Ottieni la collezione di estensioni web dal workbook
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Aggiungi una nuova estensione web (creerà l'estensione con i parametri richiesti)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Imposta la proprietà Id (poiché è leggibile e scrivibile)
                webExtension.Id = "SampleAddin123";
                
                // Visualizza il valore corrente della proprietà Id
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Modifica la proprietà Id per dimostrare che è scrivibile
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Salva la cartella di lavoro
                workbook.Save("WebExtensionIdDemo.xlsx");
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

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


