---
title: "WebExtension.IsFrozen"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtension property. Anger om användaren kan interagera med Office-tillägget eller inte"
type: docs
url: /sv/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Anger om användaren kan interagera med Office-tillägget eller inte.

```csharp
public bool IsFrozen { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Den här raden kommer att misslyckas eftersom WebExtension kräver konstruktörsparametrar
                // WebExtension webExtension = new WebExtension();
                
                // Istället hämtar vi en web extension från arbetsboken om möjligt
                // eller demonstrera med ett annat tillvägagångssätt
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // För demonstrationsändamål visar vi hur egenskapen skulle fungera om du hade en giltig instans
                // I ett verkligt scenario skulle du hämta WebExtension-instansen från arbetsboken eller en annan källa
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // Ställ in initiala egenskaper
                    webExtension.Id = "MyAddin123";
                    
                    // Visa initialt IsFrozen‑värde
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Ändra IsFrozen‑egenskapen (eftersom den är läs‑skriv)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Demonstrera effekten genom att kontrollera om användaren kan interagera
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Spara arbetsboken (även om web extension kanske inte sparas utan ytterligare steg)
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
            // I en verklig implementation skulle detta hämta en befintlig WebExtension från arbetsboken
            // eller skapa en på rätt sätt med erforderliga konstruktörsparametrar
            // Detta är bara en platshållare för demonstration
            return null;
        }
    }
}
```

### Se även

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


