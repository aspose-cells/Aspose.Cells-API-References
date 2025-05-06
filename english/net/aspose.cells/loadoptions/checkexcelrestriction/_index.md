---
title: LoadOptions.CheckExcelRestriction
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValuestring if this property is true you will get an Exception. If this property is false we will accept your input string value as the cells value so that later you can output the complete string value for other file formats such as CSV. However if you have set such kind of value that is invalid for excel file format you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file
type: docs
url: /net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Examples

```csharp
// Called: CheckExcelRestriction = true,
[Test]
        public void Property_CheckExcelRestriction()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET46794/&quot;;

            Aspose.Cells.HtmlLoadOptions htmlLoadOptions = new Aspose.Cells.HtmlLoadOptions()
            {
                CheckExcelRestriction = true,
                AutoFitColsAndRows = false,
                Encoding = Encoding.UTF8,
                SupportDivTag = false,
            };
            string html = File.ReadAllText(filePath + &quot;source - 副本.html&quot;);
            var workbook = new Workbook(new MemoryStream(Encoding.UTF8.GetBytes(html)), htmlLoadOptions);

            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;H2&quot;].IsRichText(), true);
            Assert.AreEqual(&quot;&lt;&gt;&lt;&gt;&lt;&gt;&quot;, cells[&quot;K2&quot;].StringValue);
            workbook.Save(CreateFolder(filePath) + @&quot;out.xlsx&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


