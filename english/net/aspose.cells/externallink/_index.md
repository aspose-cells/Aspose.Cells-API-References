---
title: Class ExternalLink
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalLink class. Represents an external link in a workbook
type: docs
url: /net/aspose.cells/externallink/
---
## ExternalLink class

Represents an external link in a workbook.

```csharp
public class ExternalLink
```

## Properties

| Name | Description |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Represents data source of the external link. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Indicates whether this external link is referenced by others. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Indicates whether this external link is visible in MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Represents stored data source of the external link. |
| [Type](../../aspose.cells/externallink/type/) { get; } | Gets the type of external link. |

## Methods

| Name | Description |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Adds an external name. |

### Examples

```csharp

[C#]

//Open a file with external links
Workbook workbook = new Workbook("book1.xls");

//Get External Link 
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

//Change External Link's Data Source
externalLink.DataSource = "d:\\link.xls";

[VB.NET]

'Open a file with external links
Dim workbook As New Workbook("book1.xls")

'Get External Link 
Dim externalLink As ExternalLink = workbook.Worksheets.ExternalLinks(0)

'Change External Link's Data Source
externalLink.DataSource = "d:\link.xls"
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


