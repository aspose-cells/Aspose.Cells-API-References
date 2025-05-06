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
// Called: Assert.AreEqual(&amp;quot;MyMonths&amp;quot;, pt.RowFields[1].Name);
[Test]
        public void Property_Int32_()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet54422.xlsx&quot;);
            wb.CalculateFormula();
            wb.Worksheets.RefreshAll();
            //Setting Custom Pivot Table Globalization Settings
            CustomPivotTableGlobalizationSettings settings = new CustomPivotTableGlobalizationSettings();
            //settings.SetTestMode(testMode);
            wb.Settings.GlobalizationSettings.PivotSettings = (settings);

            PivotTable pt = wb.Worksheets[0].PivotTables[0];
            DateTime start = new DateTime(2024,1,1);
            DateTime end = new DateTime(2024, 1, 15);
            //ArrayList groupTypeList = new ArrayList();
            //groupTypeList.Add(PivotGroupByType.Months);
            //groupTypeList.Add(PivotGroupByType.Years);
            // pivot.SetManualGroupField(dateBaseField, start, end, groupTypeList, 1);
            pt.RowFields[0].GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, true);
            wb.Save(Constants.PivotTableDestPath + &quot;CellsNet54422.xlsx&quot;);
            Assert.AreEqual(&quot;MyYears&quot;, pt.RowFields[0].Name);
            Assert.AreEqual(&quot;MyMonths&quot;, pt.RowFields[1].Name);
            //   pt.CalculateData();
            Assert.AreEqual(start.Year.ToString(), wb.Worksheets[0].Cells[&quot;F10&quot;].StringValue);
            Assert.AreEqual(&quot;Jan&quot;, wb.Worksheets[0].Cells[&quot;F11&quot;].StringValue);
         

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
// Called: pvtTable.RowFields[&amp;quot;Item&amp;quot;].PivotItems[&amp;quot;AAA3&amp;quot;].PositionInSameParentNode = 2;
[Test]
        public void Property_String_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43214And43215_&quot;;

            //Workbook workbook = new Workbook(filePath + &quot;pivotTable_test.xls&quot;);
            //Worksheet worksheet = workbook.Worksheets[1];
            //PivotTable table = worksheet.PivotTables[0];
            //table.ColumnFields[&quot;Continent&quot;].PivotItems[&quot;Africa&quot;].Move(-5);//move up
            //table.RowFields[&quot;Product&quot;].PivotItems[&quot;Maxilaku&quot;].Move(1);//move down
            //workbook.Save(CreateFolder(filePath) + &quot;pivotTable_test_output.xlsx&quot;);

            Workbook wb = new Workbook(filePath + @&quot;PivotTest3.xlsx&quot;);
            Worksheet wsPivot = wb.Worksheets.Add(&quot;pvtNew Hardware&quot;);
            Worksheet wsData = wb.Worksheets[&quot;New Hardware - Yearly&quot;];
            // get the pivottables collection for the pivot sheet
            PivotTableCollection pivotTables = wsPivot.PivotTables;
            // add PivotTable to the worksheet
            int index = pivotTables.Add(&quot;=&apos;New Hardware - Yearly&apos;!A1:D621&quot;, &quot;A3&quot;, &quot;HWCounts_PivotTable&quot;);
            // get the PivotTable object
            PivotTable pvtTable = pivotTables[index];
            // add vendor row field
            pvtTable.AddFieldToArea(PivotFieldType.Row, &quot;Vendor&quot;);
            // add item row field
            pvtTable.AddFieldToArea(PivotFieldType.Row, &quot;Item&quot;);
            // add data field
            pvtTable.AddFieldToArea(PivotFieldType.Data, &quot;2014&quot;);
            // turn off the subtotals for the vendor row field
            PivotField pivotField = pvtTable.RowFields[&quot;Vendor&quot;];
            pivotField.SetSubtotals(PivotFieldSubtotalType.None, true);
            // turn off grand total
            pvtTable.ShowColumnGrandTotals = false;
            // THIS ONLY SEEMS TO MOVE 4H12 DOWN BY 1 POSITION??
            //pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;4H12&quot;].Move(4);
            //Please call the PivotTable. RefreshData() and PivotTable. CalculateData() 
            //before using PivotItem.Position, PivotItem.PositionInSameParentNode  and PivotItem.Move(int count, bool isSameParent).

            pvtTable.RefreshData();
            pvtTable.CalculateData();

            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;4H12&quot;].Move(0, true);
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;DIF400&quot;].Move(-1, true);
            //As a result of using PivotItem.PositionInSameParentNode,it will change the original sort sequence,
            //so when you use PivotItem.PositionInSameParentNode in another parent node,you need call the method named &quot;CalculateData&quot; again.
            pvtTable.CalculateData();
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;CA32&quot;].Move(0, true);
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;AAA3&quot;].Move(-1, true);
            Assert.AreEqual(wsPivot.Cells[&quot;B5&quot;].StringValue, &quot;4H12&quot;);
            Assert.AreEqual(wsPivot.Cells[&quot;B6&quot;].StringValue, &quot;DIF400&quot;);
            Assert.AreEqual(wsPivot.Cells[&quot;B11&quot;].StringValue, &quot;CA32&quot;);
            Assert.AreEqual(wsPivot.Cells[&quot;B12&quot;].StringValue, &quot;KL32&quot;);
            // save file
            wb.Save(Constants.PivotTableDestPath + @&quot;NET43214And43215_PivotTest3_move_out.xlsx&quot;);

            wb = new Workbook(filePath + @&quot;PivotTest3.xlsx&quot;);
            wsPivot = wb.Worksheets.Add(&quot;pvtNew Hardware&quot;);
            wsData = wb.Worksheets[&quot;New Hardware - Yearly&quot;];
            // get the pivottables collection for the pivot sheet
            pivotTables = wsPivot.PivotTables;
            // add PivotTable to the worksheet
            index = pivotTables.Add(&quot;=&apos;New Hardware - Yearly&apos;!A1:D621&quot;, &quot;A3&quot;, &quot;HWCounts_PivotTable&quot;);
            // get the PivotTable object
            pvtTable = pivotTables[index];
            // add vendor row field
            pvtTable.AddFieldToArea(PivotFieldType.Row, &quot;Vendor&quot;);
            // add item row field
            pvtTable.AddFieldToArea(PivotFieldType.Row, &quot;Item&quot;);
            // add data field
            pvtTable.AddFieldToArea(PivotFieldType.Data, &quot;2014&quot;);
            // turn off the subtotals for the vendor row field
            pivotField = pvtTable.RowFields[&quot;Vendor&quot;];
            pivotField.SetSubtotals(PivotFieldSubtotalType.None, true);
            // turn off grand total
            pvtTable.ShowColumnGrandTotals = false;
            // THIS ONLY SEEMS TO MOVE 4H12 DOWN BY 1 POSITION??
            //pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;4H12&quot;].Move(4);
            //Please call the PivotTable. RefreshData() and PivotTable. CalculateData() 
            //before using PivotItem.Position, PivotItem.PositionInSameParentNode  and PivotItem.Move(int count, bool isSameParent).

            pvtTable.RefreshData();
            pvtTable.CalculateData();
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;4H12&quot;].PositionInSameParentNode = 1;
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;DIF400&quot;].PositionInSameParentNode = 2;
            //As a result of using PivotItem.PositionInSameParentNode,it will change the original sort sequence,
            //so when you use PivotItem.PositionInSameParentNode in another parent node,you need call the method named &quot;CalculateData&quot; again.
            pvtTable.CalculateData();
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;CA32&quot;].PositionInSameParentNode = 1;
            pvtTable.RowFields[&quot;Item&quot;].PivotItems[&quot;AAA3&quot;].PositionInSameParentNode = 2;
            Assert.AreEqual(wsPivot.Cells[&quot;B5&quot;].StringValue, &quot;4H12&quot;);
            Assert.AreEqual(wsPivot.Cells[&quot;B6&quot;].StringValue, &quot;DIF400&quot;);
            Assert.AreEqual(wsPivot.Cells[&quot;B11&quot;].StringValue, &quot;CA32&quot;);
            Assert.AreEqual(wsPivot.Cells[&quot;B12&quot;].StringValue, &quot;KL32&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET43214And43215_PivotTest3_position_out.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


