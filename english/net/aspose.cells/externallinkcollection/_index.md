---
title: Class ExternalLinkCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalLinkCollection class. Represents external links collection in a workbook
type: docs
url: /net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Represents external links collection in a workbook.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Gets the number of elements actually contained in the collection. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Gets the [`ExternalLink`](../externallink/) element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Adds an external link. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Add an external link . |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Removes all external links. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Removes all external links. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Get an enumerator that iterates through this collection. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Removes the specified external link from the workbook. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Removes the specified external link from the workbook. |

### Examples

```csharp
[C#]
//Open a file with external links
Workbook workbook = new Workbook("book1.xls");

//Change external link data source
workbook.Worksheets.ExternalLinks[0].DataSource = "d:\\link.xls";


[Visual Basic]
'Open a file with external links
Dim workbook As Workbook =  New Workbook("book1.xls")

'Change external link data source
workbook.Worksheets.ExternalLinks(0).DataSource = "d:\\link.xls"
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


