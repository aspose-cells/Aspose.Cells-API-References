---
title: WorksheetCollection.CustomDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();
workbook.Worksheets.CustomDocumentProperties.Add("Checked by", "Jane");

[Visual Basic]
Dim workbook as Workbook = New Workbook()
workbook.Worksheets.CustomDocumentProperties.Add("Checked by", "Jane")
```

### See Also

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


