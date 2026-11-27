---
title: "DocumentPropertyCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocumentPropertyCollection-egenskap. Returnerar ett DocumentProperty-objekt baserat på egenskapens namn."
type: docs
url: /sv/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Returnerar ett [`DocumentProperty`](../../documentproperty/)-objekt baserat på egenskapens namn.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Det skiftlägesokänsliga namnet på egenskapen som ska hämtas. |

### Anmärkningar

Returnerar null om en egenskap med det angivna namnet inte hittas.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string key = "TemplateGUID";
            object value = "TestValue123";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
            {
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            }
            else
            {
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
            }

            // Verifiera att värdet sattes med Item-egenskapen
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Returnerar ett [`DocumentProperty`](../../documentproperty/)-objekt baserat på index.

```csharp
public DocumentProperty this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Nollbaserat index för det [`DocumentProperty`](../../documentproperty/) som ska hämtas. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta inbyggda dokumentegenskaper
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Ställ in inbyggda egenskaper (inte Add)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Åtkomst till egenskaper med Item-indexerare
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Åtkomst till egenskap efter namn
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Ändra en egenskap
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


