---
title: HtmlLoadOptions.DeleteRedundantSpaces
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether delete redundant spaces when the text wraps lines using br tag. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. The default value is false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Examples

```csharp
// Called: ldps.DeleteRedundantSpaces = true;
[Test]
        public void Property_DeleteRedundantSpaces()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45538/&quot;;

            string savePath = CreateFolder(filePath);

            HtmlLoadOptions ldps = new HtmlLoadOptions(LoadFormat.MHtml);
           // ldps.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            ldps.DeleteRedundantSpaces = true;
            ldps.AutoFitColsAndRows = true;

            Workbook workbook = new Workbook(filePath + &quot;Original.XLS&quot;, ldps);

            workbook.Save(savePath + &quot;out.xls&quot;);
            workbook.Save(savePath + &quot;out.xlsx&quot;);
            workbook.Save(savePath + &quot;out.mht&quot;, SaveFormat.MHtml);
            Worksheet sheet = workbook.Worksheets[0];
            //sheet.AutoFitColumns();
            Assert.AreEqual(sheet.Shapes.Count, 1);
            Assert.AreEqual(sheet.Cells[&quot;A9&quot;].StringValue, &quot;NAME&quot;);
            Assert.AreEqual(sheet.Cells[&quot;A9&quot;].GetStyle().ForegroundColor, Color.FromArgb(255, 231, 243, 253));

            Assert.AreEqual(sheet.Cells[&quot;A10&quot;].GetStyle().Font.IsBold, false);
            Assert.AreEqual(sheet.Cells[&quot;G11&quot;].GetStyle().Font.IsBold, true);

            Assert.AreEqual(sheet.Cells[&quot;G11&quot;].StringValue, &quot;473.00&quot;);

            Assert.AreEqual(((CellArea)sheet.Cells.GetMergedAreas()[4]).EndColumn, 8);
            Assert.AreEqual(((CellArea)sheet.Cells.GetMergedAreas()[5]).EndColumn, 8);
            Assert.AreEqual(((CellArea)sheet.Cells.GetMergedAreas()[6]).EndColumn, 8);

        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


