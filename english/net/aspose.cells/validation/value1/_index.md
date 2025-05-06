---
title: Validation.Value1
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the first value associated with the data validation
type: docs
url: /net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Represents the first value associated with the data validation.

```csharp
public object Value1 { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(((object[])workbook.Worksheets[0].Validations[1].Value1).Length, 2);
[Test]
       public void Property_Value1()
       {
           Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET44400.xlsx&quot;);
           Assert.AreEqual(((object[])workbook.Worksheets[0].Validations[0].Value1).Length, 2);
           Assert.AreEqual(((object[])workbook.Worksheets[0].Validations[1].Value1).Length, 2);

           workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET44506.xlsx&quot;);
           Assert.AreEqual(((object[])workbook.Worksheets[0].Validations[0].Value1).Length, 4);
           Assert.AreEqual(((object[])workbook.Worksheets[0].Validations[1].Value1).Length, 5);
       }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


