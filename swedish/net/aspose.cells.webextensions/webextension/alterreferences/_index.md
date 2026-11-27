---
title: "WebExtension.AlterReferences"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtension egenskap. Hämtar en lista med alter-referenser"
type: docs
url: /sv/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Hämtar en lista över alter-referenser.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Hämta samling av web extensions från arbetsboken
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Lägg till ett nytt web extension
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Åtkomst till AlterReferences-egenskapen (skrivskyddad)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Visa information om alter-referenser
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Lägg till en ny alter-referens (demonstrerar användning av samlingen)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Visa uppdaterat antal
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Spara arbetsboken
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

### Se även

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


