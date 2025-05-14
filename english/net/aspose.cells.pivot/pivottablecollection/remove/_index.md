---
title: PivotTableCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCollection method. Deletes the specified PivotTable and delete the PivotTable data
type: docs
url: /net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Deletes the specified PivotTable and delete the PivotTable data

```csharp
public void Remove(PivotTable pivotTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |

### Examples

```csharp
// Called: pivotTables.Remove(pivotTable);
public void PivotTableCollection_Method_Remove()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46034_";

    Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(filePath + "DataSourceRemoved-2.xls");
    Worksheet sheet = workbook.Worksheets[0];
    PivotTableCollection pivotTables = sheet.PivotTables;
    PivotTable pivotTable = pivotTables[0];

    //sheet.PivotTables.Clear(); 
    //sheet.PivotTables.RemoveAt(0); 
    pivotTables.Remove(pivotTable);
    Assert.AreEqual(0, pivotTables.Count);


    workbook.Save(CreateFolder(filePath) + "out.xls");
}
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

Deletes the specified PivotTable

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |
| keepData | Boolean | Whether to keep the PivotTable data |

### Examples

```csharp
// Called: pivotsD.Remove(pivotsD[0], false);
public void PivotTableCollection_Method_Remove()
{
    string filePath = Constants.PivotTableSourcePath + @"NET48683_";
    string savePath = CreateFolder(filePath);

    Workbook wbA = new Workbook(filePath + "a.xlsx");

    PivotTableCollection pivotsA = wbA.Worksheets[0].PivotTables;
    pivotsA[0].RefreshData();
    pivotsA[0].CalculateData();
    //keep data
    pivotsA.RemoveAt(0, true);
    Assert.AreEqual(wbA.Worksheets[0].Cells["D9"].StringValue, "a1");
    wbA.Save(savePath + "a_out.xlsx");

    Workbook wbB = new Workbook(filePath + "b.xlsx");
    PivotTableCollection pivotsB = wbB.Worksheets[0].PivotTables;
    pivotsB[0].RefreshData();
    pivotsB[0].CalculateData();
    //delete data
    pivotsB.RemoveAt(0, false);
    Assert.AreEqual(wbB.Worksheets[0].Cells["D9"].StringValue, "");
    wbB.Save(savePath + "b_out.xlsx");

    Workbook wbC = new Workbook(filePath + "c.xlsx");
    PivotTableCollection pivotsC = wbC.Worksheets[0].PivotTables;
    pivotsC[0].RefreshData();
    pivotsC[0].CalculateData();
    //keep data
    pivotsC.Remove(pivotsC[0], true);
    Assert.AreEqual(wbC.Worksheets[0].Cells["D9"].StringValue, "a1");
    wbC.Save(savePath + "c_out.xlsx");

    Workbook wbD = new Workbook(filePath + "d.xlsx");
    PivotTableCollection pivotsD = wbD.Worksheets[0].PivotTables;
    pivotsD[0].RefreshData();
    pivotsD[0].CalculateData();
    //delete data
    pivotsD.Remove(pivotsD[0], false);
    Assert.AreEqual(wbD.Worksheets[0].Cells["D9"].StringValue, "");
    wbD.Save(savePath + "d_out.xlsx");

    Workbook wbE = new Workbook(filePath + "e.xlsx");
    PivotTableCollection pivotsE = wbE.Worksheets[0].PivotTables;
    pivotsE[0].RefreshData();
    pivotsE[0].CalculateData();
    //delete data
    pivotsE.Remove(pivotsE[0]);
    Assert.AreEqual(wbE.Worksheets[0].Cells["D9"].StringValue, "");
    wbD.Save(savePath + "e_out.xlsx");

    Workbook wbF = new Workbook(filePath + "f.xlsx");
    PivotTableCollection pivotsF = wbF.Worksheets[0].PivotTables;
    pivotsF[0].RefreshData();
    pivotsF[0].CalculateData();
    //delete data
    pivotsF.RemoveAt(0);
    Assert.AreEqual(wbF.Worksheets[0].Cells["D9"].StringValue, "");
    wbD.Save(savePath + "f_out.xlsx");
}
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


