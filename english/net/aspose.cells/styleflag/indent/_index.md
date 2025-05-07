---
title: StyleFlag.Indent
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Indent level setting will be applied
type: docs
url: /net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

Indent level setting will be applied.

```csharp
public bool Indent { get; set; }
```

### Examples

```csharp
// Called: var tcStyleFlag = new StyleFlag { Indent = true };
[Test]
        public void Property_Indent()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47178/";

            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            var tcStyle = ws.Workbook.CreateStyle();
            tcStyle.IndentLevel = 2;
            var tcStyleFlag = new StyleFlag { Indent = true };
            // Add some data
            for (int r = 0; r < 4; r++)
            {
                for (int c = 0; c < 4; c++)
                {
                    if (r == 0)
                    {
                        var cellValue = string.Format("Column {0}", c);
                        ws.Cells[r, c].PutValue(cellValue);
                    }
                    else
                    {
                        var cellValue = r + c;
                        ws.Cells[r, c].PutValue(cellValue);
                    }
                }
            }
            var range = ws.Cells.CreateRange(1, 0, 3, 4);
            var index = ws.ListObjects.Add(range.FirstRow - 1, range.FirstColumn, range.FirstRow + 3, range.FirstColumn + 3, true);
            ws.ListObjects[index].TableStyleType = TableStyleType.TableStyleLight16;
            range.ApplyStyle(tcStyle, tcStyleFlag);

            Style a2Style = wb.Worksheets[0].Cells["A2"].GetStyle();
            Assert.AreEqual(a2Style.IndentLevel, 2);
            Assert.AreEqual(a2Style.HorizontalAlignment, TextAlignmentType.Left);

            string savePath = CreateFolder(filePath);
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            wb.Save(savePath + "out.xls", saveOptions);
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            wb.Save(savePath + "out.html", htmlSaveOptions);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


