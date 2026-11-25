---
title: "Classe CustomPropertyCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Properties.CustomPropertyCollection. Una raccolta di oggetti CustomProperty che rappresentano informazioni aggiuntive"
type: docs
url: /it/net/aspose.cells.properties/custompropertycollection/
---
## CustomPropertyCollection class

Una raccolta di [`CustomProperty`](../customproperty/) oggetti che rappresentano informazioni aggiuntive.

```csharp
public class CustomPropertyCollection : CollectionBase<CustomProperty>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/custompropertycollection/item/) { get; } | Ottiene la proprietà personalizzata tramite l'indice specifico. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.properties/custompropertycollection/add/)(string, string) | Aggiunge informazioni sulla proprietà personalizzata. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomProperty, IComparer&lt;CustomProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomProperty, IComparer&lt;CustomProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyCollectionDemo
    {
        public static void CustomPropertyCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi al CustomPropertyCollection del foglio di lavoro
            CustomPropertyCollection customProperties = worksheet.CustomProperties;

            // Aggiungi proprietà personalizzate
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            // Accedi e stampa le proprietà personalizzate
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CustomPropertyCollectionExample.xlsx");
            workbook.Save("CustomPropertyCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomProperty](../customproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


