---
title: PivotTable.PrintDrill
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable
type: docs
url: /net/aspose.cells.pivot/pivottable/printdrill/
---
## PivotTable.PrintDrill property

Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.

```csharp
public bool PrintDrill { get; set; }
```

### Examples

```csharp
// Called: pivotTable.PrintDrill = false;
[Test]
        public void Property_PrintDrill()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45040_&quot;;

            //License lic = new License();
            //lic.SetLicense(&quot;Aspose.Total.lic&quot;);
            Workbook workbook = new Workbook(filePath + @&quot;template.xlsm&quot;);

            Worksheet selectedSheet = workbook.Worksheets[&quot;Data&quot;];
            DataTable dt = new DataTable();
            dt.ReadXml(filePath + @&quot;5874043b-a487-47cd-a7c0-5195f82fbbca.xml&quot;);
            if (dt.Rows.Count &gt; 0) selectedSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
            string pivotFormula = &quot;=&apos;Data&apos;!A1:EP2806&quot;;

            selectedSheet = workbook.Worksheets[&quot;Exposure&quot;];
            workbook.Worksheets.ActiveSheetIndex = selectedSheet.Index;
            int iIndex = selectedSheet.PivotTables.Add(pivotFormula, &quot;A7&quot;, &quot;IRIS007_pivot&quot;);
            PivotTable pivotTable = selectedSheet.PivotTables[iIndex];
            pivotTable.PivotTableStyleType = PivotTableStyleType.None;
            pivotTable.PreserveFormatting = true;
            pivotTable.ManualUpdate = true;
            pivotTable.IsAutoFormat = false;
            pivotTable.RefreshDataOnOpeningFile = false; // important for the bug
            pivotTable.MergeLabels = false;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
            pivotTable.PrintDrill = false;
            pivotTable.ShowDrill = false;
            Action&lt;PivotField&gt; setFieldSetting = (s) =&gt;
            {
                s.ShowCompact = false;
                s.IsRepeatItemLabels = false;
                s.InsertBlankRow = false;
                s.ShowAllItems = false;
                s.ShowSubtotalAtTop = false;
                s.ShowInOutlineForm = false;
            };
            iIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Expo Date Code&quot;);
            PivotField selectedField = pivotTable.ColumnFields[iIndex];
            selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
            selectedField.ShowAllItems = true;

            Action&lt;PivotField&gt; hideEmpty = (s) =&gt;
            {
                string[] items = s.Items;
                for (int iItems = 0; iItems &lt; s.ItemCount; iItems++)
                {
                    if (String.IsNullOrWhiteSpace(items[iItems])) s.HideItem(iItems, true);
                }
            };
            Action&lt;string&gt; addRow = (cell) =&gt;
            {
                iIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, cell);
                selectedField = pivotTable.RowFields[iIndex];
                selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
                selectedField.IsAutoSort = true;
                selectedField.IsAscendSort = true;
                setFieldSetting(selectedField);
            };
            addRow(&quot;Product&quot;);
            addRow(&quot;Series name&quot;);
            addRow(&quot;Synth Trade Type&quot;);
            addRow(&quot;Hedge&quot;);
            addRow(&quot;Hedge Name&quot;);
            addRow(&quot;Event Date&quot;);
            addRow(&quot;Event Status&quot;);

            iIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Expo qty&quot;);
            selectedField = pivotTable.DataFields[iIndex];
            selectedField.Function = ConsolidationFunction.Sum;
            selectedField.DisplayName = &quot;Qty&quot;;
            selectedField.NumberFormat = &quot;#,##0;[Red]-#,##0&quot;;

            pivotTable.RefreshData();
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            selectedSheet.AutoFitColumns();
            Assert.AreEqual(selectedSheet.Cells[&quot;D11&quot;].StringValue, &quot;2018285&quot;);
            workbook.Save(CreateFolder(filePath) + @&quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


