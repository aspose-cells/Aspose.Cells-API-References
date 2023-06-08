---
title: WorksheetCollection.BuiltInDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Returns a DocumentProperty collection that represents all the builtin document properties of the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Remarks

A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list:

Title

Subject

Author

Keywords

Comments

Template

Last Author

Revision Number

Application Name

Last Print Date

Creation Date

Last Save Time

Total Editing Time

Number of Pages

Number of Words

Number of Characters

Security

Category

Format

Manager

Company

Number of Bytes

Number of Lines

Number of Paragraphs

Number of Slides

Number of Notes

Number of Hidden Slides

Number of Multimedia Clips

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();
DocumentProperty doc = workbook.Worksheets.BuiltInDocumentProperties["Author"];
doc.Value = "John Smith";

[Visual Basic]
Dim workbook as Workbook = New Workbook()
Dim doc as DocumentProperty = workbook.Worksheets.BuiltInDocumentProperties("Author")
doc.Value = "John Smith"
```

### See Also

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


