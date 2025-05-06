---
title: PivotTable.CalculateData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates pivottables data to cells
type: docs
url: /net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata}

Calculates pivottable's data to cells.

```csharp
public void CalculateData()
```

### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### Examples

```csharp
// Called: pivotsA[0].CalculateData();
[Test]
        public void Method_CalculateData()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET48683_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wbA = new Workbook(filePath + &quot;a.xlsx&quot;);

            PivotTableCollection pivotsA = wbA.Worksheets[0].PivotTables;
            pivotsA[0].RefreshData();
            pivotsA[0].CalculateData();
            //keep data
            pivotsA.RemoveAt(0, true);
            Assert.AreEqual(wbA.Worksheets[0].Cells[&quot;D9&quot;].StringValue, &quot;a1&quot;);
            wbA.Save(savePath + &quot;a_out.xlsx&quot;);

            Workbook wbB = new Workbook(filePath + &quot;b.xlsx&quot;);
            PivotTableCollection pivotsB = wbB.Worksheets[0].PivotTables;
            pivotsB[0].RefreshData();
            pivotsB[0].CalculateData();
            //delete data
            pivotsB.RemoveAt(0, false);
            Assert.AreEqual(wbB.Worksheets[0].Cells[&quot;D9&quot;].StringValue, &quot;&quot;);
            wbB.Save(savePath + &quot;b_out.xlsx&quot;);

            Workbook wbC = new Workbook(filePath + &quot;c.xlsx&quot;);
            PivotTableCollection pivotsC = wbC.Worksheets[0].PivotTables;
            pivotsC[0].RefreshData();
            pivotsC[0].CalculateData();
            //keep data
            pivotsC.Remove(pivotsC[0], true);
            Assert.AreEqual(wbC.Worksheets[0].Cells[&quot;D9&quot;].StringValue, &quot;a1&quot;);
            wbC.Save(savePath + &quot;c_out.xlsx&quot;);

            Workbook wbD = new Workbook(filePath + &quot;d.xlsx&quot;);
            PivotTableCollection pivotsD = wbD.Worksheets[0].PivotTables;
            pivotsD[0].RefreshData();
            pivotsD[0].CalculateData();
            //delete data
            pivotsD.Remove(pivotsD[0], false);
            Assert.AreEqual(wbD.Worksheets[0].Cells[&quot;D9&quot;].StringValue, &quot;&quot;);
            wbD.Save(savePath + &quot;d_out.xlsx&quot;);

            Workbook wbE = new Workbook(filePath + &quot;e.xlsx&quot;);
            PivotTableCollection pivotsE = wbE.Worksheets[0].PivotTables;
            pivotsE[0].RefreshData();
            pivotsE[0].CalculateData();
            //delete data
            pivotsE.Remove(pivotsE[0]);
            Assert.AreEqual(wbE.Worksheets[0].Cells[&quot;D9&quot;].StringValue, &quot;&quot;);
            wbD.Save(savePath + &quot;e_out.xlsx&quot;);

            Workbook wbF = new Workbook(filePath + &quot;f.xlsx&quot;);
            PivotTableCollection pivotsF = wbF.Worksheets[0].PivotTables;
            pivotsF[0].RefreshData();
            pivotsF[0].CalculateData();
            //delete data
            pivotsF.RemoveAt(0);
            Assert.AreEqual(wbF.Worksheets[0].Cells[&quot;D9&quot;].StringValue, &quot;&quot;);
            wbD.Save(savePath + &quot;f_out.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata_1}

Calculating pivot tables with options

```csharp
public void CalculateData(PivotTableCalculateOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption |  |

### Examples

```csharp
// Called: pt.CalculateData(option);
[Test]
        public void Method_PivotTableCalculateOption_()
        {
            Workbook w = new Workbook(Constants.PivotTableSourcePath +  &quot;CELLSNET56086.xlsx&quot;);
            w.Worksheets[0].Cells[&quot;B3&quot;].PutValue(&quot;a&quot;);

            PivotTable pt = w.Worksheets[0].PivotTables[0];
            PivotTableCalculateOption option = new PivotTableCalculateOption();
            option.RefreshData = true;
            pt.CalculateData(option);
           Assert.AreEqual(&quot;a&quot;,w.Worksheets[0].Cells[&quot;E9&quot;].StringValue);
            w.Save(Constants.PivotTableDestPath + &quot;CELLSNET56086.xlsx&quot;);
        }
```

### See Also

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


