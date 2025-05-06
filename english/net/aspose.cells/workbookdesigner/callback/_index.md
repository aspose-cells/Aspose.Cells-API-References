---
title: WorkbookDesigner.CallBack
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Gets and sets callback interface of processing smartmarker
type: docs
url: /net/aspose.cells/workbookdesigner/callback/
---
## WorkbookDesigner.CallBack property

Gets and sets callback interface of processing smartmarker.

```csharp
public ISmartMarkerCallBack CallBack { get; set; }
```

### Examples

```csharp
// Called: designer.CallBack = b;
[Test]
        public void Property_CallBack()
        {
            var workBook = new Workbook(FileFormatType.Excel97To2003);
            var sheet = workBook.Worksheets[0];

            var dt = new DataTable(&quot;TEST&quot;);
            dt.Columns.Add(&quot;TAG_TAG1.00&quot;, typeof(string));
            dt.Columns.Add(&quot;TAG_TAG2.00&quot;, typeof(string));

            for (int i = 0; i &lt; 10; i++)
            {
                var dr = dt.NewRow();
                foreach (DataColumn item in dt.Columns)
                {
                    dr[item.ColumnName] = &quot;1000&quot;;
                }

                dt.Rows.Add(dr);
            }

            sheet.Cells[0, 0].PutValue(&quot;&amp;=[TEST].[TAG_TAG1.00](copystyle)&quot;);
            sheet.Cells[0, 1].PutValue(&quot;&amp;=[TEST].[TAG_TAG2.00](copystyle)&quot;);
            SCallBack b = new SCallBack();
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workBook
            };
            designer.CallBack = b;
            designer.SetDataSource(dt);
            designer.Process();
            Assert.AreEqual(&quot;1000&quot;, workBook.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
            workBook.Save(Constants.destPath + &quot;CellsNet47477.xlsx&quot;);
        }
```

### See Also

* interface [ISmartMarkerCallBack](../../ismartmarkercallback/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


