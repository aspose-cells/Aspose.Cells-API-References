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
// Called: Assert.AreEqual(o1.CustomProperties[&amp;quot;COR_Report&amp;quot;].Value, o2.CustomProperties[&amp;quot;COR_Report&amp;quot;].Value);
[Test]
        public void Property_Value()
        {
            var excelWorkbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-40886.xlsx&quot;);
            var o1 = excelWorkbook.Worksheets[0];


            String filePath = Constants.sourcePath + &quot;CELLSNET-40886.xls&quot;;
            Workbook xlsWorkbook = new Workbook(filePath);
            var o2 = xlsWorkbook.Worksheets[0];

            Assert.AreEqual(o1.CustomProperties[&quot;COR_Report&quot;].Value, o2.CustomProperties[&quot;COR_Report&quot;].Value);
            //{
            //    Console.WriteLine(&quot;COR_Report is equal in both files.&quot;);
            //}

            Assert.AreEqual(o1.CustomProperties[&quot;COR_ResultSet&quot;].Value, o2.CustomProperties[&quot;COR_ResultSet&quot;].Value);
            //{
            //    Console.WriteLine(&quot;COR_ResultSet is equal in both files.&quot;);
            //} 

        }
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


