---
title: ConditionalFormattingValue.Value
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValue property. Get or set the value of this conditional formatting value object. It should be used in conjunction with Type
type: docs
url: /net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Get or set the value of this conditional formatting value object. It should be used in conjunction with Type.

```csharp
public object Value { get; set; }
```

### Remarks

If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.

### Examples

```csharp
// Called: Assert.AreEqual(0, (int)icons[0].Value);
public void ConditionalFormattingValue_Property_Value()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    ConditionalFormattingValueCollection icons = workbook.Worksheets[0].ConditionalFormattings[0][0].IconSet.Cfvos;
    Assert.AreEqual(0, (int)icons[0].Value);
    Assert.AreEqual("abc", (string)icons[2].Value);

}
```

### See Also

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


