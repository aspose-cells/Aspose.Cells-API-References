---
title: "Klass DocumentPropertyCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.DocumentPropertyCollection‑klass. Bas‑klass för samlingarna BuiltInDocumentPropertyCollection och CustomDocumentPropertyCollection"
type: docs
url: /sv/net/aspose.cells.properties/documentpropertycollection/
---
## DocumentPropertyCollection class

Bas‑klass för samlingarna [`BuiltInDocumentPropertyCollection`](../builtindocumentpropertycollection/) och [`CustomDocumentPropertyCollection`](../customdocumentpropertycollection/).

```csharp
public abstract class DocumentPropertyCollection : CollectionBase<DocumentProperty>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returnerar ett [`DocumentProperty`](../documentproperty/)‑objekt efter index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returnerar ett [`DocumentProperty`](../documentproperty/)‑objekt efter egenskapens namn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/#contains_1)(string) | Returnerar true om en egenskap med det angivna namnet finns i samlingen. |
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
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/#indexof_3)(string) | Hämtar indexet för en egenskap efter namn. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Tar bort en egenskap med det angivna namnet från samlingen. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/#removeat)(int) | Tar bort en egenskap på det angivna indexet. (2 metoder) |

### Exempel

```csharp

[C#]

//Instansiera ett Workbook-objekt genom att anropa dess tomma konstruktor
Workbook workbook = new Workbook("book1.xls");
 
//Hämta en lista över alla anpassade dokumentegenskaper i Excel-filen
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Åtkomst till en anpassad dokumentegenskap genom att använda egenskapsindexet
DocumentProperty customProperty1 = customProperties[3];
 
//Åtkomst till en anpassad dokumentegenskap genom att använda egenskapsnamnet
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Instantiate a Workbook object by calling its empty constructor
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Retrieve a list of all custom document properties of the Excel file
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Accessng a custom document property by using the property index
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Accessng a custom document property by using the property name
Dim customProperty2 As DocumentProperty = customProperties("Owner")

```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DocumentProperty](../documentproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


