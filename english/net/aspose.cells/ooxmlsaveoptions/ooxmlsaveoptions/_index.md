---
title: OoxmlSaveOptions.OoxmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions constructor. Creates the options for saving office open xml file
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Creates the options for saving office open xml file.

```csharp
public OoxmlSaveOptions()
```

### Examples

```csharp
// Called: OoxmlSaveOptions so = new OoxmlSaveOptions();
[Test]
        public void OoxmlSaveOptions_Constructor()
        {
          
            DataTable dataTable = new DataTable(&quot;Table1&quot;);
            dataTable.Columns.Add(new DataColumn(&quot;Column Name?&quot;, typeof(int)));
            dataTable.Columns.Add(new DataColumn(&quot;Column &lt;$433 (Na/me)&quot;, typeof(string)));

            int[] c1 = { 1, 2, 3, 4, 5 };
            string[] c2 = { &quot;abc&quot;, &quot;def&quot;, &quot;abc123&quot;, &quot;testdata1&quot;, &quot;jkl&quot; };

            DataRow dataRow;
            for (int i = 0; i &lt; 5; i++)
            {

                dataRow = dataTable.NewRow();
                dataRow[&quot;Column Name?&quot;] = c1[i];
                dataRow[&quot;Column &lt;$433 (Na/me)&quot;] = c2[i];
                dataTable.Rows.Add(dataRow);
            }

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SmartMarker/CELLSNET45865.xlsx&quot;);

            WorkbookDesigner designer = new WorkbookDesigner();

            designer.Workbook = workbook;

            designer.SetDataSource(dataTable);

            designer.Process(true);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;B1&quot;].StringValue, c2[0]);

            workbook.Worksheets[1].Cells.ImportData(dataTable, 0, 0, new ImportTableOptions() { IsFieldNameShown = true });
            OoxmlSaveOptions so = new OoxmlSaveOptions();
            workbook.Save(Constants.destPath + &quot;CELLSNET45865.xlsx&quot;); 
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Creates the options for saving office open xml file.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Xlsx, Xltx, Xlam, Xlsm or Xltm, otherwise the saved format will be set as Xlsx automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


