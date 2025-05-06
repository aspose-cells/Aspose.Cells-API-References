---
title: Worksheet.IsGridlinesVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets a value indicating whether the gridlines are visible.Default is true
type: docs
url: /net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Gets or sets a value indicating whether the gridlines are visible.Default is true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Examples

```csharp
// Called: sheet.IsGridlinesVisible = true;
[Test]
        public void Property_IsGridlinesVisible()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47690/&quot;;
            string savePath = CreateFolder(filePath);
            string html = @&quot;&lt;table border=&quot;&quot;2px&quot;&quot;&gt;
                            &lt;tr&gt;
                            &lt;td&gt;ID&lt;/td&gt;
                            &lt;/tr&gt;
                            &lt;tr&gt;
                            &lt;td&gt;Value&lt;/td&gt;
                            &lt;/tr&gt;
                            &lt;/table&gt;&quot;;

            byte[] byteArray = Encoding.ASCII.GetBytes(html);
            MemoryStream stream = new MemoryStream(byteArray);
            Workbook workbook = new Workbook(stream);
            Worksheet sheet = workbook.Worksheets[0];
            sheet.AutoFitColumns();
            sheet.IsGridlinesVisible = true;

            workbook.Save(savePath + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


