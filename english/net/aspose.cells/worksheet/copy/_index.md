---
title: Worksheet.Copy
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Copies contents and formats from another worksheet
type: docs
url: /net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Copies contents and formats from another worksheet.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |

### Examples

```csharp
// Called: destination.Worksheets[0].Copy(source.Worksheets[0]);
[Test]
        public void Method_Worksheet_()
        {
            var source = new Workbook(Constants.sourcePath + &quot;CELLSNET44573.xlsx&quot;);
            var destination = new Workbook();
            //  destination.DefaultStyle = source.DefaultStyle;
            destination.Worksheets[0].Copy(source.Worksheets[0]);
            Cells cells = destination.Worksheets[0].Cells;
            Style style = cells[&quot;A1&quot;].GetStyle();
            Assert.AreEqual(&quot;Calibri&quot;,style.Font.Name);
            //destination.Save(path + &quot;dest.xlsx&quot;);
            Assert.AreEqual(902,destination.Worksheets[0].Shapes[0].Width);//902
            Assert.AreEqual(600, destination.Worksheets[0].Shapes[0].Height);//600
            Util.ReSave(destination, SaveFormat.Xlsx);
            //destination.Save(Constants.destPath + &quot;CELLSNET44573.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Copies contents and formats from another worksheet.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |
| copyOptions | CopyOptions |  |

### Remarks

You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.

### Examples

```csharp
// Called: newWorkbook.Worksheets[0].Copy(workbook.Worksheets[&amp;quot;Sheet1&amp;quot;], new CopyOptions { CopyNames = true });
[Test]
        public void Method_CopyOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-43083_1.xlsx&quot;);
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Copy(workbook.Worksheets[&quot;Sheet1&quot;], new CopyOptions { CopyNames = true });
            string f = newWorkbook.Worksheets[0].Cells[&quot;D10&quot;].Formula;
            Assert.AreEqual(f, &quot;=Name3&quot;);
            string expected = &quot;[CELLSNET-43083_1.xlsx]Sheet2&apos;!$C$2&quot;;
            string act = newWorkbook.Worksheets.Names[&quot;Name3&quot;].RefersTo;
            if (!act.EndsWith(expected))
            {
                Assert.Fail(&quot;Name3.RefersTo should end with &quot; + expected + &quot; but was &quot; + act);
            }
            workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-43083_2.xlsx&quot;);
            newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Copy(workbook.Worksheets[&quot;Sheet1&quot;], new CopyOptions { CopyNames = true });
            expected = &quot;Another book.xlsx&apos;!Name6&quot;;
            act = newWorkbook.Worksheets[0].Cells[&quot;D11&quot;].Formula;
            if (!act.EndsWith(expected))
            {
                Assert.Fail(&quot;D11.Formula should end with &quot; + expected + &quot; but was &quot; + act);
            }
            expected = &quot;CELLSNET-43083_2.xlsx&apos;!Table1)&quot;;
            act = newWorkbook.Worksheets[0].Cells[&quot;D12&quot;].Formula;
            if (!act.EndsWith(expected))
            {
                Assert.Fail(&quot;D12.Formula should end with &quot; + expected + &quot; but was &quot; + act);
            }
        }
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


