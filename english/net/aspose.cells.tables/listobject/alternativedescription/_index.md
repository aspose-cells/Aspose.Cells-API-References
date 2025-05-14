---
title: ListObject.AlternativeDescription
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the alternative description
type: docs
url: /net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Gets and sets the alternative description.

```csharp
public string AlternativeDescription { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("aSXADCS", table.AlternativeDescription);
public void ListObject_Property_AlternativeDescription()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    ListObject table = wb.Worksheets[0].ListObjects[0];
    Assert.AreEqual("Test", table.AlternativeText);
    Assert.AreEqual("aSXADCS", table.AlternativeDescription);
    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    table = wb.Worksheets[0].ListObjects[0];
    Assert.AreEqual("Test", table.AlternativeText);
    Assert.AreEqual("aSXADCS", table.AlternativeDescription);
    wb.Save(Constants.destPath + "example.xlsb");
    wb = new Workbook(Constants.destPath + "example.xlsb");
    table = wb.Worksheets[0].ListObjects[0];
    Assert.AreEqual("Test", table.AlternativeText);
    Assert.AreEqual("aSXADCS", table.AlternativeDescription);
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


