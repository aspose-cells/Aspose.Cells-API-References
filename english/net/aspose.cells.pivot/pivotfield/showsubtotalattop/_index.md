---
title: PivotField.ShowSubtotalAtTop
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. when ShowInOutlineForm is true then display subtotals at the top of the list of items instead of at the bottom
type: docs
url: /net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Remarks

Only works when ShowInOutlineForm is true.

### Examples

```csharp
// Called: selectedField.ShowSubtotalAtTop = true;
[Test]
        public void Property_ShowSubtotalAtTop()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45627_&quot;;

            //Instantiating an Workbook object
            Workbook workbook = new Workbook(filePath + &quot;RPNL063.xlsx&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;Data&quot;];
            DataTable dt = new DataTable();
            dt.ReadXml(filePath + &quot;e1ff3057-8648-4f96-bd64-0f19aa60e3dd.xml&quot;);
            sheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
            sheet = workbook.Worksheets[&quot;PNL&quot;];
            ///*
            //m_pivotTable = m_excel.CreatePivotTable(&quot;RPNL063_pivot&quot;, &quot;A5&quot;, &quot;=&apos;Data&apos;!A1:AK4&quot;, false, false, false, 0);
            //
            int index = sheet.PivotTables.Add(&quot;=&apos;Data&apos;!A1:AK4&quot;, &quot;A5&quot;, &quot;RPNL063_pivot&quot;);
            PivotTable pivot = sheet.PivotTables[index];
            index = pivot.AddFieldToArea(PivotFieldType.Column, &quot;Realization Type&quot;);
            PivotField selectedField = pivot.ColumnFields[index];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
            //
            //m_pivotTable.SetFieldLayout(true, true, false, false, false, true);
            //*/
            selectedField.ShowCompact = true;
            selectedField.ShowSubtotalAtTop = true;
            selectedField.IsRepeatItemLabels = false;
            selectedField.InsertBlankRow = false;
            selectedField.ShowAllItems = false;
            selectedField.ShowInOutlineForm = true;
            index = pivot.AddFieldToArea(PivotFieldType.Column, &quot;Period&quot;);
            selectedField = pivot.ColumnFields[index];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
            index = pivot.AddFieldToArea(PivotFieldType.Row, &quot;Sub Matrix Code&quot;);
            selectedField = pivot.RowFields[index];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
            index = pivot.AddFieldToArea(PivotFieldType.Row, &quot;Hedge&quot;);
            selectedField = pivot.RowFields[index];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
            index = pivot.AddFieldToArea(PivotFieldType.Data, &quot;Currency Amount&quot;);
            pivot.ShowRowGrandTotals = false;
            pivot.RefreshData();
            pivot.CalculateRange();
            pivot.CalculateData();
            workbook.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


