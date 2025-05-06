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
// Called: Assert.AreEqual(&amp;quot;15.0300&amp;quot;, workbook.Worksheets.BuiltInDocumentProperties[&amp;quot;Version&amp;quot;].ToString());
[Test]
        public void Method_ToString()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-43355.xlsx&quot;);
            Assert.AreEqual(&quot;15.0300&quot;, workbook.Worksheets.BuiltInDocumentProperties[&quot;Version&quot;].ToString());
            workbook.Save(Constants.destPath + &quot;CELLSNET43355.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET43355.xls&quot;);
            Assert.AreEqual(&quot;15.0300&quot;, workbook.Worksheets.BuiltInDocumentProperties[&quot;Version&quot;].ToString());
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


