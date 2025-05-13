---
title: DocumentProperty.ToString
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty method. Returns the property value as a string
type: docs
url: /net/aspose.cells.properties/documentproperty/tostring/
---
## DocumentProperty.ToString method

Returns the property value as a string.

```csharp
public override string ToString()
```

### Remarks

Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.

### Examples

```csharp
// Called: Assert.AreEqual("15.0300", workbook.Worksheets.BuiltInDocumentProperties["Version"].ToString());
public void DocumentProperty_Method_ToString()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("15.0300", workbook.Worksheets.BuiltInDocumentProperties["Version"].ToString());
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual("15.0300", workbook.Worksheets.BuiltInDocumentProperties["Version"].ToString());
}
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


