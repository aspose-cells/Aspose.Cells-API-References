---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentPropertyCollection-method. Hämtar indexet för en egenskap efter namn"
type: docs
url: /sv/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Hämtar indexet för en egenskap efter namn.

```csharp
public int IndexOf(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Det skiftlägesokänsliga namnet på egenskapen. |

### Returvärde

Det nollbaserade indexet. Negativt värde om inte hittad.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta samlingen med inbyggda dokumentegenskaper
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // För inbyggda egenskaper kan vi bara sätta värden för befintliga egenskaper
            // För att lägga till anpassade egenskaper måste vi använda CustomDocumentPropertyCollection
            // Här sätter vi bara några befintliga inbyggda egenskaper för demonstration
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // Anropa IndexOf-metoden med en strängparameter
                int index = properties.IndexOf("Subject");
                
                // Visa resultatet
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Visa egenskapen på det hittade indexet
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### Se även

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


