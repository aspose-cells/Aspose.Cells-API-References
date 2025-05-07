---
title: PivotFieldCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection property. Gets the PivotField Object at the specific index
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Gets the PivotField Object at the specific index.

```csharp
public PivotField this[int index] { get; }
```

### Examples

```csharp
// Called: PivotField firstField = columnFields[0];
[Test]
        public void Property_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET47037_";

            Workbook wb = new Workbook(filePath + "SampleData.xlsx");

            PivotTable pivot = wb.Worksheets[1].PivotTables[0];
            pivot.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField pageField = pivot.PageFields[0];
            pageField.CurrentPageItem = 0;

            PivotFieldCollection columnFields = pivot.ColumnFields;
            PivotField firstField = columnFields[0];
            firstField.HideItemDetail(2, false);

            pivot.RefreshData();
            pivot.CalculateData();

            Cells cells = wb.Worksheets[1].Cells;
            Assert.AreEqual(cells["H7"].StringValue, "3");
            Assert.AreEqual(cells["H8"].StringValue, "4");
            Assert.AreEqual(cells["H9"].StringValue, "3");
            Assert.AreEqual(cells["H10"].StringValue, "2");
            Assert.AreEqual(cells["H11"].StringValue, "1");
            Assert.AreEqual(cells["H12"].StringValue, "1");
            Assert.AreEqual(cells["H13"].StringValue, "14");
            wb.Save(CreateFolder(filePath) + "out.xls");
            wb.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Gets the PivotField Object of the specific name.

```csharp
public PivotField this[string name] { get; }
```

### Examples

```csharp
// Called: int indSlicerLA = wsLASumPiv.Slicers.Add(pivotTable, "E7", pivotTable.BaseFields["Year"]);
[Test]
        public void Property_String_()
        {
            LoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            Workbook book = new Workbook(Constants.PivotTableSourcePath + "CellsNet54396.csv", loadOptions);
            book.Worksheets[0].Name = "LA_SUM";
            //Build Pivot table and Pivot Chart
            Aspose.Cells.Range rngAllData = book.Worksheets[0].Cells.MaxDisplayRange;
            Worksheet wsLASumPiv = book.Worksheets.Add("LA_SUM_Pivot");
            PivotTableCollection pivotTables = wsLASumPiv.PivotTables;
            string sourceDataPT = String.Format("=LA_SUM!{0}", rngAllData.Address);
            int indPivTab = pivotTables.Add(sourceDataPT, "A2", "PivotTbl");
            PivotTable pivotTable = pivotTables[indPivTab];

            int indSlicerYrs = wsLASumPiv.Slicers.Add(pivotTable, "E2", pivotTable.BaseFields["LA_Name"]);
            Slicer slicerYrs = wsLASumPiv.Slicers[indSlicerYrs];
            int indSlicerLA = wsLASumPiv.Slicers.Add(pivotTable, "E7", pivotTable.BaseFields["Year"]);
            Slicer slicerLA = wsLASumPiv.Slicers[indSlicerLA];

           Assert.AreEqual(4,slicerLA.SlicerCache.SlicerCacheItems.Count);
            book.Save(Constants.PivotTableDestPath + "CellsNet54396.xlsx");
        }
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


