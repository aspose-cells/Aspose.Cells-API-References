---
title: PivotTableCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCollection method. Deletes the PivotTable at the specified index and delete the PivotTable data
type: docs
url: /net/aspose.cells.pivot/pivottablecollection/removeat/
---
## RemoveAt(int) {#removeat}

Deletes the PivotTable at the specified index and delete the PivotTable data

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the position index in PivotTable collection |

### Examples

```csharp
// Called: sheet.PivotTables.RemoveAt(2);
[Test]
        public void Method_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43362_";

            Workbook workbook = new Workbook(filePath + "a.xlsx");
            Worksheet sheet = workbook.Worksheets[0];
            PivotTableCollection pivotTables = sheet.PivotTables;
            PivotTable pt0 = pivotTables[0];
            PivotTable pt1 = pivotTables[1];
            PivotTable pt2 = pivotTables[2];

            //sheet.PivotTables.Clear();
            sheet.PivotTables.RemoveAt(2);
            //sheet.PivotTables.RemoveAt(1);
            //sheet.PivotTables.RemoveAt(0);
            pivotTables.Remove(pt0);
            //pivotTables.Remove(pt1);
            //pivotTables.Remove(pt2);
            Assert.AreEqual(sheet.Cells["G12"].StringValue, "");
            Assert.AreEqual(sheet.Cells["D20"].StringValue, "");
            sheet.Charts[0].RefreshPivotData();
            sheet.Charts[1].RefreshPivotData();

            workbook.Save(Constants.PivotTableDestPath + @"NET43362.xlsx");

            workbook = new Aspose.Cells.Workbook(filePath + "Pivot.xlsx");
            sheet = workbook.Worksheets[0];
            pivotTables = sheet.PivotTables;
            PivotTable pivotTable = pivotTables[0];
            //workbook.Worksheets.ClearPivots();
            // sheet.PivotTables.Clear();
            //sheet.PivotTables.RemoveAt(0);
            pivotTables.Remove(pivotTable);
            Assert.AreEqual(sheet.PivotTables.Count, 0);
            Assert.AreEqual(sheet.Cells["D8"].StringValue, "");
            Assert.AreEqual(sheet.Cells["E8"].StringValue, "");
            workbook.Save(Constants.PivotTableDestPath + @"NET43362_Pivot_out.xlsx");
        }
```

### See Also

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_2}

Deletes the PivotTable at the specified index

```csharp
public void RemoveAt(int index, bool keepData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the position index in PivotTable collection |
| keepData | Boolean | Whether to keep the PivotTable data |

### Examples

```csharp
// Called: pivotsB.RemoveAt(0, false);
[Test]
        public void Method_Boolean_()
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

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


