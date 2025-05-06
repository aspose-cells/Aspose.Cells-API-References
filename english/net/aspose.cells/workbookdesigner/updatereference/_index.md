---
title: WorkbookDesigner.UpdateReference
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates if references in other worksheets will be updated
type: docs
url: /net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Indicates if references in other worksheets will be updated.

```csharp
public bool UpdateReference { get; set; }
```

### Examples

```csharp
// Called: designer.UpdateReference = true;
[Test]
        public void Property_UpdateReference()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            //designer.Open(Constants.sourcePath + &quot;Test_201963.xls&quot;);
            designer.Workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/Test_201963.xls&quot;);

            DataSet ds = new DataSet();
            DataTable dt = new DataTable(&quot;dataset27548&quot;);
            dt.Columns.Add(&quot;C1&quot;, typeof(string));
            dt.Columns.Add(&quot;C2&quot;, typeof(string));
            dt.Columns.Add(&quot;C3&quot;, typeof(int));
            dt.Columns.Add(&quot;C4&quot;, typeof(int));
            dt.Columns.Add(&quot;C5&quot;, typeof(double));
            dt.Columns.Add(&quot;C6&quot;, typeof(int));
            dt.Columns.Add(&quot;C7&quot;, typeof(double));
            ds.Tables.Add(dt);

            dt.Rows.Add(new object[] { &quot;A&quot;, &quot;B1&quot;, 2492609, 798, 57.3253284636968, 419, 109.178071871193 });
            dt.Rows.Add(new object[] { &quot;A&quot;, &quot;B2&quot;, 1, 798, 57.3253284636968, 419, 109.178071871193 });
            dt.Rows.Add(new object[] { &quot;A&quot;, &quot;B3&quot;, 16377681, 798, 57.3253284636968, 419, 109.178071871193 });

            designer.SetDataSource(ds);
            designer.Process(true);

            //Save the excel file
           // designer.Workbook.Settings.ConvertNumericData = true;
            designer.Workbook.CalculateFormula();
            designer.Workbook.Settings.FormulaSettings.CalculateOnOpen = true;
            designer.Workbook.Settings.FormulaSettings.CalculateOnSave = true;
            designer.UpdateReference = true;
            designer.Workbook.Save(Constants.destPath + &quot;Test_201963.xls&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


