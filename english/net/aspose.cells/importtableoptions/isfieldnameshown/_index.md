---
title: ImportTableOptions.IsFieldNameShown
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether field name should be imported
type: docs
url: /net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Indicates whether field name should be imported.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Examples

```csharp
// Called: wsheet1.Cells.ImportData(dt, sheet1StartIndex, 0, new ImportTableOptions() { IsFieldNameShown = false, InsertRows = true });
[Test]
        public void Property_IsFieldNameShown()
        {
            string TemplatePath = Constants.sourcePath + &quot;CELLSNET46873.xlsx&quot;;
            string ReportPath = Constants.destPath + &quot;CELLSNET46873.xlsx&quot;;
            Workbook wbook = new Workbook(TemplatePath);

            Worksheet wsheet1 = wbook.Worksheets[&quot;Sheet1&quot;];
            int sheet1StartIndex = 3;
            DataTable dt = GetDataForIssue_1();

            wsheet1.Cells.ImportData(dt, sheet1StartIndex, 0, new ImportTableOptions() { IsFieldNameShown = false, InsertRows = true });
            wsheet1.Cells.DeleteRows(sheet1StartIndex + dt.Rows.Count, 2);//Deleting the default rows that were there in template to provide formulae.

            wbook.Worksheets.ActiveSheetIndex = 0;
            int fileNumber = 1;
            Assert.AreEqual(&quot;=ROUND(IF(B4&lt;&gt;0,B4/$C$11,0),8)&quot;, wsheet1.Cells[&quot;C4&quot;].Formula);
            wbook.Save(ReportPath);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


