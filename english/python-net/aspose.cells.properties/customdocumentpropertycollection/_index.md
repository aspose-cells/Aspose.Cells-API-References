---
title: CustomDocumentPropertyCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---

## CustomDocumentPropertyCollection class

A collection of custom document properties.



**Inheritance:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/python-net/aspose.cells.properties/documentpropertycollection)



The CustomDocumentPropertyCollection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Gets or sets the number of elements that the array list can contain. |


### Methods
| Method | Description |
| :- | :- |
| [index_of(name)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Gets the index of a property by name. |
| [index_of(item, index)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [index_of(item, index, count)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [copy_to(array)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [copy_to(index, array, array_index, count)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [last_index_of(item)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [last_index_of(item, index)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [last_index_of(item, index, count)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [add(name, value)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Creates a new custom document property of the **PropertyType.String**  data type. |
| [add(name, value)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Creates a new custom document property of the **PropertyType.Number**  data type. |
| [add(name, value)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Creates a new custom document property of the **PropertyType.DateTime**  data type. |
| [add(name, value)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Creates a new custom document property of the **PropertyType.Boolean**  data type. |
| [add(name, value)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Creates a new custom document property of the **PropertyType.Float**  data type. |
| [binary_search(item)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
| [add_link_to_content(name, source)](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Creates a new custom document property which links to content. |
| [update_linked_property_value()](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) | Update custom document property value which links to content. |
| [update_linked_range()](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Update custom document property value to linked range. |



### Remarks 


Each [DocumentProperty](/cells/python-net/aspose.cells.properties/documentproperty) object represents a custom property of a container document.

### Example 


```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```
### See Also

* module [aspose.cells.properties](../)
* class [DocumentPropertyCollection](/cells/python-net/aspose.cells.properties/documentpropertycollection)
