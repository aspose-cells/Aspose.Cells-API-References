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
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47690/";
            string savePath = CreateFolder(filePath);
            string html = @"<table border=""2px"">
                            <tr>
                            <td>ID</td>
                            </tr>
                            <tr>
                            <td>Value</td>
                            </tr>
                            </table>";

            byte[] byteArray = Encoding.ASCII.GetBytes(html);
            MemoryStream stream = new MemoryStream(byteArray);
            Workbook workbook = new Workbook(stream);
            Worksheet sheet = workbook.Worksheets[0];
            sheet.AutoFitColumns();
            sheet.IsGridlinesVisible = true;

            workbook.Save(savePath + "out.xlsx");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


