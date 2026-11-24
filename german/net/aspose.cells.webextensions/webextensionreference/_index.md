---
title: "Klasse WebExtensionReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionReference Klasse. Stellt die Identifizierung des Anbieterspeicherorts und der Version der Erweiterung dar."
type: docs
url: /de/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Stellt die Identifizierung des Anbieters, des Speicherorts und der Version der Erweiterung dar.

```csharp
public class WebExtensionReference
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Liest und schreibt den Bezeichner, der dem Office-Add-in innerhalb eines Kataloganbieters zugeordnet ist. Der Bezeichner MUSS innerhalb eines Kataloganbieters eindeutig sein. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Liest und schreibt die Instanz des Marktplatzes, in dem das Office-Add-in gespeichert ist. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Liest und schreibt den Typ des Marktplatzes, den das Store-Attribut identifiziert. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Liest und schreibt die Version. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle zuerst eine WebExtension
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Hole die WebExtensionReference von der WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Setze Eigenschaften der WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Zeige die Referenzeigenschaften an
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


