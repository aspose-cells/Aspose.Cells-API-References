---
title: Worksheet.CustomProperties
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets an object representing the identifier information associated with a worksheet
type: docs
url: /net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Gets an object representing the identifier information associated with a worksheet.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Remarks

Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

### Examples

```csharp
// Called: Assert.AreEqual(2,copy.Worksheets[0].CustomProperties.Count);
public void Worksheet_Property_CustomProperties()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsm");
    Workbook copy = new Workbook();
    copy.Copy(wb);
    Assert.AreEqual(2,copy.Worksheets[0].CustomProperties.Count);
    Util.ReSave(copy, SaveFormat.Xlsm);
    //copy.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


