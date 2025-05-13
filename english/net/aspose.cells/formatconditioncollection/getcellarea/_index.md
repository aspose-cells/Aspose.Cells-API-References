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
public void FormatConditionCollection_Method_GetCellArea()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
   Assert.AreEqual(7,workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
    Assert.AreEqual("=She.et1!$E$3:$G$5", workbook.Worksheets.Names[0].RefersTo);
    Assert.AreEqual("=She.et1!$C$15:$E$16", workbook.Worksheets.Names[1].RefersTo);
    Assert.AreEqual("She.et1", workbook.Worksheets[1].Hyperlinks[0].Address);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.AreEqual(7, workbook.Worksheets[0].ConditionalFormattings[0].GetCellArea(0).EndRow);
    Assert.AreEqual("=She.et1!$E$3:$G$5", workbook.Worksheets.Names[0].RefersTo);
    Assert.AreEqual("=She.et1!$C$15:$E$16", workbook.Worksheets.Names[1].RefersTo);
    Assert.AreEqual("She.et1", workbook.Worksheets[1].Hyperlinks[0].Address);
    workbook.Save(Constants.destPath + "example.ods");
    using (FileStream fs = File.OpenRead(Constants.destPath + "example.ods"))
    {
        ZipFile zipFile = ZipFile.Read(fs);
        ZipEntry en = zipFile.GetEntry("content.xml");
        System.IO.Stream s = zipFile.GetInputStream(en);
        StreamReader rdr = new StreamReader(s, Encoding.UTF8);
        String text = rdr.ReadToEnd();
        Assert.AreEqual(-1, text.IndexOf("\"She.et1.B3\""));
        Assert.IsTrue(text.IndexOf("xlink:href=\"#She.et1\"") != -1);//CELLSNET-49013
    }
               
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


