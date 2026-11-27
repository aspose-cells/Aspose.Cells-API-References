---
title: "WebExtensionPropertyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionPropertyCollection-egenskap. Hämtar egenskapen för webbutökning efter index"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Hämtar egenskapen för webbutökning efter index.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Egenskapen för webbutökning.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en samling av webbutökningsegenskaper
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Lägg till några egenskaper
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Åtkomst till egenskaper med Item-indexerare
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Ändra egenskapsvärden via samlingen
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Visa förändringarna
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Spara arbetsboken (men webbutökningsegenskaper kommer inte att vara synliga i den sparade filen utan korrekt konfiguration)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Hämtar egenskapen för webbutökning.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på egenskapen. |

### Returvärde

Egenskapen för webbutökning.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en samling av webbutökningsegenskaper
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Lägg till egenskaper i samlingen
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Åtkomst till egenskaper med Item-indexeraren
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Ändra egenskapsvärden (obs: Item är skrivskyddad, så vi måste använda Add/Remove)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Visa uppdaterat värde
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Spara arbetsboken
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


