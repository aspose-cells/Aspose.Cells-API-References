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
// Called: sheet.Validations[0].Formula1 = &amp;quot;=B1:B2&amp;quot;;
[Test]
       public void Property_Formula1()
       {
           Workbook workbook = new Workbook(FileFormatType.Xlsx);
           Worksheet sheet = workbook.Worksheets[0];
           sheet.Validations.Add(CellArea.CreateCellArea(&quot;A1&quot;,&quot;A1&quot;));
           sheet.Validations[0].Type = ValidationType.List;
           sheet.Validations[0].Formula1 = &quot;=B1:B2&quot;;
           sheet.Cells[&quot;B1&quot;].PutValue(&quot;A&quot;);
           sheet.Cells[&quot;B2&quot;].PutValue(&quot;B&quot;);
           object t = sheet.Validations[0].Value1;
           Assert.AreEqual(&quot;A&quot;, ((object[])t)[0].ToString());
       }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


