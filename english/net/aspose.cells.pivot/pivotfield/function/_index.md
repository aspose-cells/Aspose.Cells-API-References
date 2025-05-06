---
title: PivotField.Function
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the function used to summarize the PivotTable data field
type: docs
url: /net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Represents the function used to summarize the PivotTable data field.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Examples

```csharp
// Called: selectedField.Function = Aspose.Cells.ConsolidationFunction.Sum;
[Test]
        public void Property_Function()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44090_&quot;;
           
            File.Copy(filePath + @&quot;bug_template.xlsb&quot;, Constants.PivotTableDestPath + @&quot;NET44090result.xlsb&quot;, true);
            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.PivotTableDestPath + @&quot;NET44090result.xlsb&quot;);
            Aspose.Cells.Worksheet workSheet = workbook.Worksheets[&quot;Data&quot;];
            DataSet ds = new DataSet();
            ds.ReadXmlSchema(filePath + @&quot;schema.xml&quot;);
            ds.ReadXml(filePath + @&quot;data.xml&quot;);
            DataTable dt = ds.Tables[&quot;DataTable&quot;];
            workSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
            string strFormula = String.Format(@&quot;={0}!{1}:{2}&quot;, workSheet.Name, Aspose.Cells.CellsHelper.CellIndexToName(0, 0),
                Aspose.Cells.CellsHelper.CellIndexToName(workSheet.Cells.MaxDataRow, workSheet.Cells.MaxDataColumn));
            workSheet = workbook.Worksheets[&quot;Exposure&quot;];
            Aspose.Cells.Pivot.PivotTableCollection pivotTables = workSheet.PivotTables;
            int iIndex = pivotTables.Add(strFormula, &quot;A5&quot;, &quot;RIRI_LOULOU_FIFI&quot;);
            Aspose.Cells.Pivot.PivotTable pivot = pivotTables[iIndex];
            iIndex = pivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, &quot;Underlying Expo Date Code&quot;);
            Aspose.Cells.Pivot.PivotField selectedField = pivot.ColumnFields[iIndex];
            selectedField.IsAutoSort = true;
            selectedField.IsAscendSort = true;
            selectedField.DisplayName = &quot;Underlying Expo Date Code&quot;;
            iIndex = pivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Synth Trade Type&quot;);
            selectedField = pivot.RowFields[iIndex];
            selectedField.IsAutoSort = true;
            selectedField.IsAscendSort = true;
            iIndex = pivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Product name&quot;);
            selectedField = pivot.RowFields[iIndex];
            selectedField.IsAutoSort = true;
            selectedField.IsAscendSort = true;
            iIndex = pivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Synth Series Name&quot;);
            selectedField = pivot.RowFields[iIndex];
            selectedField.IsAutoSort = true;
            selectedField.IsAscendSort = true;
            iIndex = pivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;Expo qty&quot;);
            selectedField = pivot.DataFields[iIndex];
            selectedField.DisplayName = &quot;Qty&quot;;
            selectedField.Function = Aspose.Cells.ConsolidationFunction.Sum;
            pivot.CalculateRange();
            pivot.CalculateData();
            workbook.Worksheets.ActiveSheetIndex = workSheet.Index;
            workbook.Save(Constants.PivotTableDestPath + @&quot;NET44090out.xlsb&quot;);
        }
```

### See Also

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


