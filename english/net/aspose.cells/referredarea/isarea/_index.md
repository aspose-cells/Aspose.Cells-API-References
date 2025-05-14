---
title: ReferredArea.IsArea
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates whether this is an area
type: docs
url: /net/aspose.cells/referredarea/isarea/
---
## ReferredArea.IsArea property

Indicates whether this is an area.

```csharp
public bool IsArea { get; }
```

### Remarks

If this is not an area, only StartRow and StartColumn effect.

### Examples

```csharp
// Called: if (ra.IsArea != (i == 0))
public void ReferredArea_Property_IsArea()
{
    Workbook wb = new Workbook();
    wb.Worksheets[0].Cells[3, 3].PutValue("v03");
    Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
    n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
    Aspose.Cells.Range[] rs = n.GetRanges(true);
    if (rs == null)
    {
        Assert.Fail("GetRanges should not return null");
    }
    else if (rs.Length != 1)
    {
        Assert.Fail("GetRanges gives incorrect count of ranges: " + rs.Length);
    }
    else
    {
        if (rs[0].RowCount > 1 || rs[0].ColumnCount > 1)
        {
            Assert.Fail("Got range should be single");
        }
        if (rs[0].FirstRow != 3 || rs[0].FirstColumn != 3)
        {
            Assert.Fail("Incorrect address for returned Range: "
                + CellsHelper.CellIndexToName(rs[0].FirstRow, rs[0].FirstColumn));
        }
    }
    ReferredArea[] ras = n.GetReferredAreas(true);
    if (ras == null)
    {
        Assert.Fail("GetReferredAreas should not return null");
    }
    if (ras.Length != 4)
    {
        Assert.Fail("GetReferredAreas gives incorrect count of areas: " + ras.Length);
    }
    for (int i = 0; i < ras.Length; i++)
    {
        ReferredArea ra = ras[i];
        if (i == 2)
        {
            if (ra.IsExternalLink)
            {
                Assert.Fail("Areas[2] should not be ExternalLink");
            }
        }
        else
        {
            if (!ra.IsExternalLink)
            {
                Assert.Fail(i + ": should be ExternalLink");
            }
            if ("C:\\extlink" + (i == 1 ? 2 : 1) + ".xlsx" != ra.ExternalFileName)
            {
                Assert.Fail(i + ": Incorrect value of ExternalFileName[" + ra.ExternalFileName + "]");
            }
        }
        if("Sheet" + (i==1 ? 2 : 1) != ra.SheetName)
        {
            Assert.Fail(i + ": Incorrect value of SheetName[" + ra.SheetName + "]");
        }
        if (ra.IsArea != (i == 0))
        {
            Assert.Fail(i + ": Incorrect value of IsArea[" + ra.IsArea + "]");
        }
        if (i == 0)
        {
            if (ra.StartRow != 0 || ra.StartColumn != 0 || ra.EndRow != 1 || ra.EndColumn != 1)
            {
                Assert.Fail(i + ": Incorrect area[" + CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)
                    + ":" + CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn) + "]");
            }
        }
        else
        {
            if (ra.StartRow != i + 1 || ra.StartColumn != i + 1)
            {
                Assert.Fail(i + ": Incorrect address[" + CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn) + "]");
            }
        }
    }
    Workbook wb1 = new Workbook();
    wb1.FileName = "C:\\extlink1.xlsx";
    Cells cells = wb1.Worksheets[0].Cells;
    for (int i = 0; i < 5; i++)
    {
        cells[i, i].PutValue("v1" + i);
    }
    wb.UpdateLinkedDataSource(new Workbook[]{wb1});
    Assert.AreEqual("v10", ras[0].GetValue(0, 0));
    Assert.AreEqual("v11", ras[0].GetValue(1, 1));
    Assert.AreEqual("#REF!", ras[1].GetValue(0, 0));
    Assert.AreEqual("v03", ras[2].GetValue(0, 0));
    Assert.AreEqual("v14", ras[3].GetValue(0, 0));
}
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


