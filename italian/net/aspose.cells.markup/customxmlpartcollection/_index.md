---
title: "Classe CustomXmlPartCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Markup.CustomXmlPartCollection classe. Rappresenta una parte di archiviazione dati XML personalizzata all'interno di un pacchetto"
type: docs
url: /it/net/aspose.cells.markup/customxmlpartcollection/
---
## CustomXmlPartCollection class

Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto).

```csharp
public class CustomXmlPartCollection : CollectionBase<CustomXmlPart>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/customxmlpartcollection/item/) { get; } | Ottiene un elemento all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.markup/customxmlpartcollection/add/)(byte[], byte[]) | Aggiunge un elemento alla collezione. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomXmlPart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomXmlPart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SelectByID](../../aspose.cells.markup/customxmlpartcollection/selectbyid/)(string) | Ottiene un elemento per ID. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassCustomXmlPartCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni la CustomXmlPartCollection dalla cartella di lavoro
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;

            // Crea dati XML di esempio e schema
            byte[] xmlData = System.Text.Encoding.UTF8.GetBytes("<root><item>Test</item></root>");
            byte[] schemaData = System.Text.Encoding.UTF8.GetBytes("<xsd:schema xmlns:xsd='http://www.w3.org/2001/XMLSchema'></xsd:schema>");

            // Aggiungi una nuova parte XML personalizzata
            int index = customXmlParts.Add(xmlData, schemaData);

            // Ottieni la parte XML aggiunta per indice
            CustomXmlPart part = customXmlParts[index];

            // Seleziona la parte XML per ID (se noto)
            string partId = part.ID;
            CustomXmlPart selectedPart = customXmlParts.SelectByID(partId);

            // Aggiungi un'altra parte XML
            byte[] xmlData2 = System.Text.Encoding.UTF8.GetBytes("<data><value>123</value></data>");
            customXmlParts.Add(xmlData2, null);

            // Visualizza il conteggio delle parti XML personalizzate
            Console.WriteLine("Custom XML parts count: " + customXmlParts.Count);

            // Salva la cartella di lavoro
            workbook.Save("CustomXmlPartCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomXmlPart](../customxmlpart/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


