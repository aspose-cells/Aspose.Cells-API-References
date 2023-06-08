---
title: Class Hyperlink
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Hyperlink class. Encapsulates the object that represents a hyperlink
type: docs
url: /net/aspose.cells/hyperlink/
---
## Hyperlink class

Encapsulates the object that represents a hyperlink.

```csharp
public class Hyperlink
```

## Properties

| Name | Description |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Represents the address of a hyperlink. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Gets the range of hyperlink. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Gets the link type. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Returns or sets the ScreenTip text for the specified hyperlink. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |

## Methods

| Name | Description |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Deletes this hyperlink |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Workbook object
workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];
//Adding a hyperlink to a URL at "A1" cell
int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
//Getting a Hyperlink by index.
Hyperlink hyperlink = worksheet.Hyperlinks[index];
//Setting display text of this hyperlink.
hyperlink.TextToDisplay = "Aspose";
//Saving the Excel file
workbook.Save("book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Workbook object
workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Adding a hyperlink to a URL at "A1" cell
Dim index as Integer = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")
'Getting a Hyperlink by index.
Dim hyperlink as Hyperlink = worksheet.Hyperlinks(index);
'Setting display text of this hyperlink.
hyperlink.TextToDisplay = "Aspose";
'Saving the Excel file
workbook.Save("book1.xls")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


