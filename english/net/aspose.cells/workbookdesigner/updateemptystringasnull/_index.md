---
title: WorkbookDesigner.UpdateEmptyStringAsNull
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. If TRUE Null will be inserted if the value is 
type: docs
url: /net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

If TRUE, Null will be inserted if the value is "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Examples

```csharp
// Called: designer.UpdateEmptyStringAsNull = true; // new property afer Aspose version 2018.10
[Test]
        public void Property_UpdateEmptyStringAsNull()
        {
            DataTable dtStudent = new DataTable(&quot;Student&quot;);
            DataColumn dcName = new DataColumn(&quot;Name&quot;, typeof(string));
            DataColumn dcClass = new DataColumn(&quot;Class&quot;, typeof(string));
            DataColumn dcBooks = new DataColumn(&quot;Books&quot;, typeof(int));
            DataColumn dcPrice = new DataColumn(&quot;Price&quot;, typeof(double));
            DataColumn dcDate = new DataColumn(&quot;Date&quot;, typeof(DateTime));
            dtStudent.Columns.Add(dcName);
            dtStudent.Columns.Add(dcClass);
            dtStudent.Columns.Add(dcBooks);
            dtStudent.Columns.Add(dcPrice);
            dtStudent.Columns.Add(dcDate);
            // Add three rows to it
            DataRow drName1 = dtStudent.NewRow();
            DataRow drName2 = dtStudent.NewRow();
            DataRow drName3 = dtStudent.NewRow();
            DataRow drName4 = dtStudent.NewRow();

            drName1[&quot;Name&quot;] = &quot;John&quot;;
            drName2[&quot;Name&quot;] = &quot;Jack&quot;;
            drName3[&quot;Name&quot;] = &quot;James&quot;;
            drName4[&quot;Name&quot;] = &quot;Sam&quot;;
            drName1[&quot;Class&quot;] = &quot;Class1&quot;;
            drName2[&quot;Class&quot;] = &quot;Class2&quot;;
            drName3[&quot;Class&quot;] = &quot;Class1&quot;;
            drName4[&quot;Class&quot;] = &quot;Class2&quot;;
            drName1[&quot;Books&quot;] = 1;
            drName2[&quot;Books&quot;] = 2;
            drName3[&quot;Books&quot;] = 3;
            drName4[&quot;Books&quot;] = 4;
            drName1[&quot;Price&quot;] = 1.1;
            drName2[&quot;Price&quot;] = 2.2;
            drName3[&quot;Price&quot;] = 3.3;
            drName4[&quot;Price&quot;] = 4.4;
            drName1[&quot;Date&quot;] = DateTime.Now.Date;
            drName2[&quot;Date&quot;] = DateTime.Now.Date.AddDays(1);
            drName3[&quot;Date&quot;] = DateTime.Now.Date.AddDays(2);
            drName4[&quot;Date&quot;] = DateTime.Now.Date.AddDays(3);
            dtStudent.Rows.Add(drName1);
            dtStudent.Rows.Add(drName2);
            dtStudent.Rows.Add(drName3);
            dtStudent.Rows.Add(drName4);
            // The memoryPreference generates outlines in the output ,which is not expected.
            Workbook workbook = new Workbook(Constants.sourcePath + @&quot;N46820.xlsx&quot;
                , new LoadOptions() { MemorySetting = MemorySetting.MemoryPreference });

            WorkbookDesigner designer = new WorkbookDesigner();
            designer.UpdateReference = true;
            designer.UpdateEmptyStringAsNull = true; // new property afer Aspose version 2018.10
            designer.Workbook = workbook;
            DataView dv = new DataView(dtStudent);
            dv.Sort = &quot;Class&quot;;
            designer.SetDataSource(&quot;Student&quot;, dv);
            designer.Process();
            Assert.AreEqual(0, workbook.Worksheets[0].Cells.Rows[9].GroupLevel, &quot;Row.OutlineLevel&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


