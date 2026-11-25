---
title: "Classe WebExtensionReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionReference. Rappresenta l'identificazione della posizione del provider e della versione dell'estensione"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Rappresenta l'identificazione della posizione del provider e della versione dell'estensione.

```csharp
public class WebExtensionReference
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Ottiene e imposta l'identificatore associato all'Office Add-in all'interno di un provider di catalogo. L'identificatore DEVE essere unico all'interno di un provider di catalogo. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Ottiene e imposta l'istanza del marketplace in cui è archiviato l'Office Add-in. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Ottiene e imposta il tipo di marketplace che l'attributo store identifica. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Ottiene e imposta la versione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea prima un WebExtension
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Ottieni il WebExtensionReference dal WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Imposta le proprietà del WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Visualizza le proprietà di riferimento
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Salva la cartella di lavoro
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


