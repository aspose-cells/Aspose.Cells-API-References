---
title: CustomProperty.Value
second_title: Aspose.Cells for .NET API Reference
description: CustomProperty property. Returns or sets the value of the custom property
type: docs
url: /net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Returns or sets the value of the custom property.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(t, workbook.Worksheets[0].CustomProperties["VeryLongString"].Value);
public void CustomProperty_Property_Value()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    string t = workbook.Worksheets[0].CustomProperties["VeryLongString"].Value;
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(t, workbook.Worksheets[0].CustomProperties["VeryLongString"].Value);

}
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


