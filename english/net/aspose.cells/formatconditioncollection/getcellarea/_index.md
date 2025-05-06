---
title: FormatConditionCollection.GetCellArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Gets the conditional formatted cell range by index
type: docs
url: /net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

Gets the conditional formatted cell range by index.

```csharp
public CellArea GetCellArea(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the conditional formatted cell range. |

### Return Value

the conditional formatted cell range

### Examples

```csharp
// Called: Assert.AreEqual(7,workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET49014.xlsx&quot;);
           Assert.AreEqual(7,workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
            Assert.AreEqual(&quot;=She.et1!$E$3:$G$5&quot;, workbook.Worksheets.Names[0].RefersTo);
            Assert.AreEqual(&quot;=She.et1!$C$15:$E$16&quot;, workbook.Worksheets.Names[1].RefersTo);
            Assert.AreEqual(&quot;She.et1&quot;, workbook.Worksheets[1].Hyperlinks[0].Address);
            workbook.Save(Constants.destPath + &quot;CELLSNET49014.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET49014.ods&quot;);
            Assert.AreEqual(7, workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
            Assert.AreEqual(&quot;=She.et1!$E$3:$G$5&quot;, workbook.Worksheets.Names[0].RefersTo);
            Assert.AreEqual(&quot;=She.et1!$C$15:$E$16&quot;, workbook.Worksheets.Names[1].RefersTo);
            Assert.AreEqual(&quot;She.et1&quot;, workbook.Worksheets[1].Hyperlinks[0].Address);
            workbook.Save(Constants.destPath + &quot;CELLSNET49014.ods&quot;);
            using (FileStream fs = File.OpenRead(Constants.destPath + &quot;CELLSNET49014.ods&quot;))
            {
                ZipFile zipFile = ZipFile.Read(fs);
                ZipEntry en = zipFile.GetEntry(&quot;content.xml&quot;);
                System.IO.Stream s = zipFile.GetInputStream(en);
                StreamReader rdr = new StreamReader(s, Encoding.UTF8);
                String text = rdr.ReadToEnd();
                Assert.AreEqual(-1, text.IndexOf(&quot;\&quot;She.et1.B3\&quot;&quot;));
                Assert.IsTrue(text.IndexOf(&quot;xlink:href=\&quot;#She.et1\&quot;&quot;) != -1);//CELLSNET-49013
            }
               
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


