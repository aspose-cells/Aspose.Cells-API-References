---
title: PivotField.SetSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specified field shows that subtotals
type: docs
url: /net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Sets whether the specified field shows that subtotals.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | subtotals type. |
| shown | Boolean | whether the specified field shows that subtotals. |

### Examples

```csharp
// Called: selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
[Test]
        public void Method_Boolean_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45267_&quot;;

            Workbook workbook = new Workbook(filePath + @&quot;Template.xlsm&quot;);
            Worksheet selectedSheet = workbook.Worksheets[&quot;Data&quot;];
            DataTable dt = new DataTable();
            dt.ReadXml(filePath + @&quot;8d828882-2028-4b9e-9aa6-074a53a58cda.xml&quot;);
            selectedSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
            selectedSheet = workbook.Worksheets[&quot;Exposure&quot;];
            int iIndex = selectedSheet.PivotTables.Add(&quot;=&apos;Data&apos;!A1:EQ15042&quot;, &quot;A7&quot;, &quot;IRIS007_pivot&quot;);
            PivotTable selectedPivotTable = selectedSheet.PivotTables[iIndex];
            selectedPivotTable.RefreshDataOnOpeningFile = false; // important we need it

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Expo Date Code&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Series name&quot;);
            PivotField selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Trade Type&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Put/Call&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Strike Price&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge Name&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;B/S&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Event&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Event Date&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Event Status&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Formula&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Position Product Code&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            /* the row field we would like to correctly format */
            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Position Qty&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
            selectedField.NumberFormat = &quot;[Blue]#,##0;[Red]-#,##0&quot;;

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Pricing Dates&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Inco Term&quot;);
            selectedField = selectedPivotTable.RowFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Expo qty&quot;);
            selectedField = selectedPivotTable.DataFields[iIndex];
            selectedField.NumberFormat = &quot;#,##0;[Red]-#,##0&quot;;

            selectedPivotTable.RefreshData();
            selectedPivotTable.CalculateRange();
            selectedPivotTable.CalculateData();
            Assert.AreEqual(selectedSheet.Cells[&quot;M13&quot;].StringValue, &quot;2,550&quot;);
            Assert.AreEqual(selectedSheet.Cells[&quot;M13&quot;].GetDisplayStyle().Font.Color, Color.FromArgb(255, 0, 0, 255));
            Assert.AreEqual(selectedSheet.Cells[&quot;M14&quot;].StringValue, &quot;-5,250&quot;);
            Assert.AreEqual(selectedSheet.Cells[&quot;M14&quot;].GetDisplayStyle().Font.Color, Color.FromArgb(255, 255, 0, 0));

            workbook.Save(CreateFolder(filePath) + @&quot;out.xlsm&quot;);
        }
```

### See Also

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


