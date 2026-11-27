---
title: "DocumentPropertyCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentPropertyCollection-metod. Tar bort en egenskap på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.properties/documentpropertycollection/removeat/
---
## DocumentPropertyCollection.RemoveAt method

Tar bort en egenskap på det angivna indexet.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Det nollbaserade indexet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till anpassade dokumentegenskaper (istället för inbyggda)
            DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Lägg till några anpassade egenskaper för att demonstrera borttagning
            ((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
            ((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
            ((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");

            try
            {
                // Visa egenskaper före borttagning
                Console.WriteLine("Properties before removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                // Anropa RemoveAt med index 1 (andra egenskapen)
                properties.RemoveAt(1);

                // Visa egenskaper efter borttagning
                Console.WriteLine("\nProperties after removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                Console.WriteLine("RemoveAt method executed successfully with parameter (Int32)");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error: Index out of range. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("RemoveAtMethodDemo.xlsx");
        }
    }
}
```

### Se även

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


