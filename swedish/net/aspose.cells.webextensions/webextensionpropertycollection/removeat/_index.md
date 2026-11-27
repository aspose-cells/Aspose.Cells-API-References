---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionPropertyCollection-metod. Ta bort egenskapen efter namn."
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Ta bort egenskapen efter namn.

```csharp
public void RemoveAt(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en samling av webbutökningsegenskaper
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Lägg till några egenskaper i samlingen
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // Anropa RemoveAt-metoden med en strängparameter
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Visa återstående egenskaper
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


