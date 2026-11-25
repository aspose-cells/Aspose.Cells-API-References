---
title: "Classe DocumentPropertyCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Properties.DocumentPropertyCollection class. Classe base per le raccolte BuiltInDocumentPropertyCollection e CustomDocumentPropertyCollection"
type: docs
url: /it/net/aspose.cells.properties/documentpropertycollection/
---
## DocumentPropertyCollection class

Classe base per le raccolte [`BuiltInDocumentPropertyCollection`](../builtindocumentpropertycollection/) e [`CustomDocumentPropertyCollection`](../customdocumentpropertycollection/).

```csharp
public abstract class DocumentPropertyCollection : CollectionBase<DocumentProperty>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Restituisce un oggetto [`DocumentProperty`](../documentproperty/) per indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Restituisce un oggetto [`DocumentProperty`](../documentproperty/) per nome della proprietà. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/#contains_1)(string) | Restituisce true se una proprietà con il nome specificato esiste nella raccolta. |
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
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/#indexof_3)(string) | Ottiene l'indice di una proprietà per nome. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Rimuove una proprietà con il nome specificato dalla raccolta. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/#removeat)(int) | Rimuove una proprietà all'indice specificato. (2 metodi) |

### Esempi

```csharp

[C#]

//Istanzia un oggetto Workbook chiamando il suo costruttore vuoto
Workbook workbook = new Workbook("book1.xls");
 
//Recupera un elenco di tutte le proprietà personalizzate del documento Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Accesso a una proprietà del documento personalizzata usando l'indice della proprietà
DocumentProperty customProperty1 = customProperties[3];
 
//Accesso a una proprietà del documento personalizzata usando il nome della proprietà
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

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DocumentProperty](../documentproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


