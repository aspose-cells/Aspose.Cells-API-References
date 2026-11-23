---
title: "Classe DocumentPropertyCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Properties.DocumentPropertyCollection class. Classe de base pour les collections BuiltInDocumentPropertyCollection et CustomDocumentPropertyCollection"
type: docs
url: /fr/net/aspose.cells.properties/documentpropertycollection/
---
## DocumentPropertyCollection class

Classe de base pour les collections [`BuiltInDocumentPropertyCollection`](../builtindocumentpropertycollection/) et [`CustomDocumentPropertyCollection`](../customdocumentpropertycollection/).

```csharp
public abstract class DocumentPropertyCollection : CollectionBase<DocumentProperty>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Renvoie un objet [`DocumentProperty`](../documentproperty/) par indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Renvoie un objet [`DocumentProperty`](../documentproperty/) par le nom de la propriété. |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/#contains_1)(string) | Renvoie true si une propriété portant le nom spécifié existe dans la collection. |
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
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/#indexof_3)(string) | Obtient l'indice d'une propriété par son nom. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Supprime une propriété portant le nom spécifié de la collection. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/#removeat)(int) | Supprime une propriété à l'indice spécifié. (2 méthodes) |

### Exemples

```csharp

[C#]

//Instancier un objet Workbook en appelant son constructeur vide
Workbook workbook = new Workbook("book1.xls");
 
//Récupérer une liste de toutes les propriétés personnalisées du document Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Accéder à une propriété personnalisée en utilisant l'indice de la propriété
DocumentProperty customProperty1 = customProperties[3];
 
//Accéder à une propriété personnalisée en utilisant le nom de la propriété
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

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DocumentProperty](../documentproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


