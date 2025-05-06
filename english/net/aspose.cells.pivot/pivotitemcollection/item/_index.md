---
title: PivotItemCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotItemCollection property. Gets the PivotItem Object at the specific index
type: docs
url: /net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

Gets the PivotItem Object at the specific index.

```csharp
public PivotItem this[int index] { get; }
```

### Examples

```csharp
// Called: PivotItem item = pivotField.PivotItems[i];
[Test]
        public void Property_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47335_&quot;;

            Workbook workbook = new Workbook(filePath + &quot;Filter.xlsx&quot;);
            PivotTable table = workbook.Worksheets[0].PivotTables[0];
            PivotField pivotField = table.PageFields[0];

            pivotField.IsMultipleItemSelectionAllowed = true;

            int pageItemCount = pivotField.PivotItems.Count;
            //Select a, e, i, oitems only 
            for (int i = 0; i &lt; pageItemCount; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                switch (item.Name)
                {
                    case &quot;a&quot;:
                    case &quot;e&quot;:
                    case &quot;i&quot;:
                    case &quot;o&quot;:
                        item.IsHidden = false;
                        break;
                    default:
                        item.IsHidden = true;
                        break;
                }
            }

            table.RefreshData();
            table.CalculateData();

            workbook.Save(CreateFolder(filePath) + &quot;filter_out.xlsx&quot;);

            Workbook wb = new Workbook(filePath + &quot;To Aspose.xlsx&quot;);
            Worksheet sheet = wb.Worksheets.Add(&quot;Test&quot;);
            int pivotIndex = sheet.PivotTables.Add(&quot;=ExportPOC2_AggregateData7_M!$A$1:$D$24&quot;, &quot;A3&quot;, &quot;TestPivot&quot;);
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 3);

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;

            pivot.RefreshData();
            pivot.CalculateData();

            PivotConditionalFormatCollection pfcc = pivot.ConditionalFormats;
            int pIndex = pfcc.Add();
            PivotConditionalFormat pfc = pfcc[pIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            CellArea dataBodyRange = pivot.DataBodyRange;

            string startCell = CellsHelper.CellIndexToName(dataBodyRange.StartRow, dataBodyRange.StartColumn);
            fcc.AddArea(dataBodyRange);

            //you can add other format conditions
            //now we will replace 1 with &quot;Direct&quot;
            int idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = &quot;=&quot; + startCell + &quot;=1&quot;;
            fc.Operator = OperatorType.Equal;
            fc.Style.Custom = &quot;[=1]\&quot;Direct\&quot;;;&quot;;

            //replace 8 with &quot;Direct8&quot;
            idx = fcc.AddCondition(FormatConditionType.Expression);
            fc = fcc[idx];
            fc.Formula1 = &quot;=&quot; + startCell + &quot;=8&quot;;
            fc.Operator = OperatorType.Equal;
            fc.Style.Custom = &quot;[=8]\&quot;Direct8\&quot;;;&quot;;


            wb.Save(CreateFolder(filePath) + &quot;ToAspose_out.xlsx&quot;);
        }
```

### See Also

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

Gets the [`PivotItem`](../../pivotitem/) by the specific name.

```csharp
public PivotItem this[string itemValue] { get; }
```

### Examples

```csharp
// Called: pvtTable.RowFields[&amp;quot;Item&amp;quot;].PivotItems[&amp;quot;AAA3&amp;quot;].Move(-1, true);
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

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


