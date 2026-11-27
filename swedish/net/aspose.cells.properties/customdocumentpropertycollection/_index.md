---
title: "Klass CustomDocumentPropertyCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.CustomDocumentPropertyCollection-klass. En samling av anpassade dokumentegenskaper"
type: docs
url: /sv/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

En samling av anpassade dokumentegenskaper.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returnerar ett [`DocumentProperty`](../documentproperty/)‑objekt efter index. (Ärvd från [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returnerar ett [`DocumentProperty`](../documentproperty/)-objekt efter egenskapens namn.(Ärvd från [`DocumentPropertyCollection`](../documentpropertycollection/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add)(string, bool) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Boolean**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_3)(string, DateTime) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.DateTime**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_1)(string, double) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Float**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_2)(string, int) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Number**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_4)(string, string) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.String**. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/)(string, string) | Skapar en ny anpassad dokumentegenskap som länkar till innehåll. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/)(string) | Returnerar true om en egenskap med det angivna namnet finns i samlingen.(Ärvd från [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DocumentProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DocumentProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty) |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/)(string) | Hämtar indexet för en egenskap efter namn.(Ärvd från [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Tar bort en egenskap med det angivna namnet från samlingen.(Ärvd från [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/)(int) | Tar bort en egenskap på det angivna indexet. (2 metoder) |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/)() | Uppdaterar värden för alla anpassade egenskaper som är länkade till innehåll(use cellvärdet i det länkade området för att uppdatera värdet för den anpassade egenskapen). |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/)() | Uppdaterar alla områden som är länkade till anpassade egenskaper(use värdet av den anpassade dokumentegenskapen för att uppdatera cellvärdet i det länkade området). |

### Anmärkningar

Varje [`DocumentProperty`](../documentproperty/) objekt representerar en anpassad egenskap i ett behållardokument.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomDocumentPropertyCollectionDemo
    {
        public static void CustomDocumentPropertyCollectionExample()
        {
            // Instansiera ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämta en lista över alla anpassade dokumentegenskaper i Excel-filen
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Lägg till anpassade dokumentegenskaper
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Lägg till en länkad anpassad dokumentegenskap
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Uppdatera länkade egenskapsvärden
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Åtkomst till anpassade dokumentegenskaper
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Skriv ut anpassade dokumentegenskaper
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Spara arbetsboken
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
    }
}
```

### Se även

* class [DocumentPropertyCollection](../documentpropertycollection/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


