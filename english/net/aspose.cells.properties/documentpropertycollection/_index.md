---
title: Class DocumentPropertyCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Properties.DocumentPropertyCollection class. Base class for BuiltInDocumentPropertyCollection and CustomDocumentPropertyCollection collections
type: docs
url: /net/aspose.cells.properties/documentpropertycollection/
---
## DocumentPropertyCollection class

Base class for [`BuiltInDocumentPropertyCollection`](../builtindocumentpropertycollection/) and [`CustomDocumentPropertyCollection`](../customdocumentpropertycollection/) collections.

```csharp
public abstract class DocumentPropertyCollection : CollectionBase<DocumentProperty>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returns a [`DocumentProperty`](../documentproperty/) object by index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Returns a [`DocumentProperty`](../documentproperty/) object by the name of the property. |

## Methods

| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/#contains_1)(string) | Returns true if a property with the specified name exists in the collection. |
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
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/#indexof_3)(string) | Gets the index of a property by name. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Removes a property with the specified name from the collection. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/#removeat)(int) | Removes a property at the specified index. (2 methods) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionDemo
    {
        public static void DocumentPropertyCollectionExample()
        {
            //// Instantiate a Workbook object by calling its empty constructor
            //Workbook workbook = new Workbook("DocumentPropertyCollection_original.xlsx");

            //// Retrieve a list of all custom document properties of the Excel file
            //DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            //// Accessing a custom document property by using the property index
            //DocumentProperty customProperty1 = customProperties[3];
            //Console.WriteLine($"Property Name: {customProperty1.Name}, Property Value: {customProperty1.Value}");

            //// Accessing a custom document property by using the property name
            //DocumentProperty customProperty2 = customProperties["Owner"];
            //Console.WriteLine($"Property Name: {customProperty2.Name}, Property Value: {customProperty2.Value}");

            //// Check if a custom property exists
            //bool containsProperty = customProperties.Contains("Owner");
            //Console.WriteLine($"Contains 'Owner' property: {containsProperty}");

            //// Get the index of a custom property
            //int propertyIndex = customProperties.IndexOf("Owner");
            //Console.WriteLine($"Index of 'Owner' property: {propertyIndex}");

            //// Remove a custom property by name
            //customProperties.Remove("Owner");

            //// Remove a custom property by index
            //customProperties.RemoveAt(3);

            //// Set the capacity of the custom properties collection
            //customProperties.Capacity = 10;
            //Console.WriteLine($"Capacity of custom properties: {customProperties.Capacity}");

            //// Get the count of custom properties
            //int count = customProperties.Count;
            //Console.WriteLine($"Count of custom properties: {count}");

            //// Save the workbook
            //workbook.Save("DocumentPropertyCollectionExample.xlsx");
            //workbook.Save("DocumentPropertyCollectionExample.pdf");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DocumentProperty](../documentproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


