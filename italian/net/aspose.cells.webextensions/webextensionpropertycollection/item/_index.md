---
title: "WebExtensionPropertyCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionPropertyCollection. Ottiene la proprietà della web extension per indice"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Ottiene la proprietà della web extension per indice.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La proprietà della web extension.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Creare una raccolta di proprietà web extension
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Aggiungi alcune proprietà
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Accedi alle proprietà usando l'indicizzatore Item
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Modifica i valori delle proprietà tramite la collezione
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Dimostra le modifiche
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Salva la cartella di lavoro (anche se le proprietà dell'estensione web non saranno visibili nel file salvato senza una configurazione adeguata)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Ottiene la proprietà dell'estensione web.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della proprietà. |

### Valore di ritorno

La proprietà della web extension.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Creare una raccolta di proprietà web extension
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Aggiunge proprietà alla collezione
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Accedi alle proprietà usando l'indicizzatore Item
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Modifica i valori delle proprietà (nota: Item è di sola lettura, quindi è necessario usare Aggiungi/Rimuovi)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Mostra il valore aggiornato
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Salva la cartella di lavoro
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


