---
title: Validation.Formula1
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the value or expression associated with the data validation
type: docs
url: /net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Represents the value or expression associated with the data validation.

```csharp
public string Formula1 { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("A,B,C", workbook.Worksheets[0].Validations[0].Formula1);
public void Validation_Property_Formula1()
{

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("A,B,C", workbook.Worksheets[0].Validations[0].Formula1);
    Assert.AreEqual("=A5", workbook.Worksheets[0].Validations[1].Formula1);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.AreEqual("A,B,C", workbook.Worksheets[0].Validations[0].Formula1);
    Assert.AreEqual("=A5", workbook.Worksheets[0].Validations[1].Formula1);
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "example.ods", "content.xml", new string[] { "of:is-true-formula([.A5])", "of:cell-content-is-in-list(&quot;A&quot;;&quot;B&quot;;&quot;C&quot;)" }, true));
           

}
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


