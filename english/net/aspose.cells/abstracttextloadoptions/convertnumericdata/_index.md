---
title: AbstractTextLoadOptions.ConvertNumericData
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to numeric data
type: docs
url: /net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

```csharp
public bool ConvertNumericData { get; set; }
```

### Examples

```csharp
// Called: loadOptions.ConvertNumericData = true;
[Test]
        public void Property_ConvertNumericData()
        {
            string html = @" 
            <table data-cache=""not-cached"" class=""sortable""> 
                <tbody> 
                    <tr> 
                        <td class=""even"">999999999999999999</td> 
                        <td class=""odd"">10.8%</td> 
                    </tr> 
                </tbody> 
            </table> 
        ";

            byte[] byteArray = Encoding.UTF8.GetBytes(html);
            HtmlLoadOptions loadOptions = new Aspose.Cells.HtmlLoadOptions(LoadFormat.Html);
            loadOptions.ConvertNumericData = true;
            loadOptions.KeepPrecision = true;
            MemoryStream stream = new MemoryStream(byteArray);
            Workbook workbook = new Workbook(stream, loadOptions);
            Worksheet sheet = workbook.Worksheets[0];


            sheet.AutoFitColumns();

            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "999999999999999999");
        }
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


