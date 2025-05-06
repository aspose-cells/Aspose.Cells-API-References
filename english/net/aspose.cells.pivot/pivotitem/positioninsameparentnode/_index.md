---
title: PivotItem.PositionInSameParentNode
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Specifying the position index in the PivotItems under the same parent node
type: docs
url: /net/aspose.cells.pivot/pivotitem/positioninsameparentnode/
---
## PivotItem.PositionInSameParentNode property

Specifying the position index in the PivotItems under the same parent node.

```csharp
public int PositionInSameParentNode { get; set; }
```

### Examples

```csharp
// Called: pvtTable.RowFields[&amp;quot;Item&amp;quot;].PivotItems[&amp;quot;4H12&amp;quot;].PositionInSameParentNode = 1;
[Test]
        public void Property_PositionInSameParentNode()
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

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


