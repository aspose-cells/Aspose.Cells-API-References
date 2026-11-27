---
title: "SmartTagPropertyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagPropertyCollection‑egenskap. Hämtar ett SmartTagProperty‑objekt"
type: docs
url: /sv/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Hämtar ett [`SmartTagProperty`](../../smarttagproperty/)‑objekt.

```csharp
public SmartTagProperty this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet |

### Returvärde

Returnerar ett [`SmartTagProperty`](../../smarttagproperty/)‑objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en samling av smarta tagg‑egenskaper
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Lägg till egenskaper i samlingen
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Åtkomst till egenskaper med Item-indexerare
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Visa aktuella egenskapsvärden
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Obs: Item‑egenskapen är skrivskyddad, så vi kan inte tilldela den direkt
            // Istället kan vi modifiera egenskaperna hos de returnerade SmartTagProperty‑objekten
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Visa uppdaterade värden
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Spara arbetsboken (även om smarta taggar inte lagras synligt vid en enkel sparning)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Hämtar ett [`SmartTagProperty`](../../smarttagproperty/)‑objekt efter egenskapens namn.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på egenskapen. |

### Returvärde

Returnerar ett [`SmartTagProperty`](../../smarttagproperty/)‑objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en smart tag‑inställning och lägg till en smart tagg
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Hämta smart taggen och dess egenskaper
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Lägg till några egenskaper för att demonstrera Item‑egenskapen
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Åtkomst till egenskaper med Item-indexeraren (efter index)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Visa egenskapsvärdena
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Spara arbetsboken
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
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

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


