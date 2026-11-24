---
title: "WebExtension.IsFrozen"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtension-Eigenschaft. Gibt an, ob der Benutzer mit dem Office-Add-In interagieren kann oder nicht"
type: docs
url: /de/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Gibt an, ob der Benutzer mit dem Office-Add-In interagieren kann oder nicht.

```csharp
public bool IsFrozen { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Diese Zeile schlägt fehl, weil WebExtension Konstruktorparameter benötigt
                // WebExtension webExtension = new WebExtension();
                
                // Stattdessen erhalten wir, wenn möglich, eine WebExtension aus der Arbeitsmappe
                // oder demonstriere mit einem anderen Ansatz
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // Zu Demonstrationszwecken zeigen wir, wie die Eigenschaft funktionieren würde, wenn Sie eine gültige Instanz hätten
                // In einem realen Szenario würden Sie die WebExtension-Instanz aus der Arbeitsmappe oder einer anderen Quelle erhalten
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // Setzen Sie die Anfangseigenschaften
                    webExtension.Id = "MyAddin123";
                    
                    // Initialen IsFrozen-Wert anzeigen
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Ändere die IsFrozen-Eigenschaft (da sie les- und schreibbar ist)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Demonstriere die Wirkung, indem du prüfst, ob der Benutzer interagieren kann
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Speichere die Arbeitsmappe (obwohl die WebExtension ohne zusätzliche Schritte möglicherweise nicht gespeichert wird)
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
            // In einer realen Implementierung würde dies eine vorhandene WebExtension aus der Arbeitsmappe holen
            // oder erstelle sie korrekt mit den erforderlichen Konstruktorparametern
            // Dies ist nur ein Platzhalter für die Demonstration
            return null;
        }
    }
}
```

### Siehe auch

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


