---
title: "SmartTagPropertyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagPropertyCollection. Ottiene un oggetto SmartTagProperty"
type: docs
url: /it/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Ottiene un oggetto [`SmartTagProperty`](../../smarttagproperty/).

```csharp
public SmartTagProperty this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice |

### Valore di ritorno

Restituisce un oggetto [`SmartTagProperty`](../../smarttagproperty/).

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una raccolta di proprietà del tag intelligente
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Aggiunge proprietà alla collezione
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Accedi alle proprietà usando l'indicizzatore Item
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Visualizza i valori correnti delle proprietà
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Nota: la proprietà Item è di sola lettura, quindi non possiamo assegnarle direttamente
            // Invece, possiamo modificare le proprietà degli oggetti SmartTagProperty restituiti
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Visualizza i valori aggiornati
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Salva la cartella di lavoro (anche se i tag intelligenti non vengono memorizzati visibilmente in un salvataggio semplice)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Ottiene un oggetto [`SmartTagProperty`](../../smarttagproperty/) in base al nome della proprietà.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della proprietà. |

### Valore di ritorno

Restituisce un oggetto [`SmartTagProperty`](../../smarttagproperty/).

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un'impostazione di tag intelligente e aggiungi un tag intelligente
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Ottieni il tag intelligente e le sue proprietà
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Aggiungi alcune proprietà per dimostrare la proprietà Item
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Accedi alle proprietà usando l'indicizzatore Item (per indice)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Visualizza i valori delle proprietà
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


