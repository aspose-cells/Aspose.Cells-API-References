---
title: "WebExtension.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtension egenskap. Hämtar och sätter den unika identifieraren för Office Addin-instansen i det aktuella dokumentet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Hämtar och anger den unika identifieraren för Office-tilläggets instans i det aktuella dokumentet.

```csharp
public string Id { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Hämta samling av web extensions från arbetsboken
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Lägg till en ny web extension (detta kommer att skapa den med nödvändiga parametrar)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Ange Id-egenskapen (eftersom den är läs-/skrivbar)
                webExtension.Id = "SampleAddin123";
                
                // Visa det aktuella värdet för Id-egenskapen
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Ändra Id-egenskapen för att demonstrera att den är skrivbar
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Spara arbetsboken
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

### Se även

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


