---
title: WorksheetCollection.RegisterAddInFunction
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Adds addin function into the workbook
type: docs
url: /net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Adds addin function into the workbook

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | String | the file contains the addin functions |
| functionName | String | the addin function name |
| lib | Boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |

### Return Value

ID of the data which contains given addin function

### Examples

```csharp
// Called: int id = wb.Worksheets.RegisterAddInFunction(addInFileRel, &amp;quot;TEST_UDF&amp;quot;, false);
private void Method_Boolean_(string ext)
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 16.0);
            string addInFileRel = &quot;..\\..\\..\\template\\Formula\\AddIn1.xlam&quot;;
            string addInFileAbs = Path.GetFullPath(Constants.sourcePath + &quot;Formula\\AddIn2.xlam&quot;);
            int id = wb.Worksheets.RegisterAddInFunction(addInFileRel, &quot;TEST_UDF&quot;, false);
            wb.Worksheets.RegisterAddInFunction(id, &quot;TEST_UDF1&quot;);
            wb.Worksheets.RegisterAddInFunction(addInFileAbs, &quot;TEST_UDF&quot;, false);
            Util.SetHintMessage(cells[0, 0], &quot;Before AddIn files being loaded(Macros should also be enabled), all formulas are Error values(#NAME! and error messages)&quot;);
            Util.SetHintMessage(cells[1, 0], &quot;After loading [&quot; + addInFileRel + &quot;], A5:B7 should have no error&quot;);
            Util.SetHintMessage(cells[2, 0], &quot;After loading [&quot; + addInFileAbs + &quot;], A8:B9 should have no error&quot;);
            cells[4, 0].Formula = &quot;=&apos;&quot; + addInFileRel + &quot;&apos;!TEST_UDF()&quot;;
            cells[4, 1].Formula = &quot;=IF(IFERROR(A5,\&quot;Error\&quot;)=\&quot;UDF000\&quot;,\&quot;OK\&quot;,\&quot;Expect UDF000\&quot;)&quot;;
            cells[5, 0].Formula = &quot;=&apos;&quot; + addInFileRel + &quot;&apos;!TEST_UDF()&amp;TEST_UDF1()&quot;;
            cells[5, 1].Formula = &quot;=IF(IFERROR(A6,\&quot;Error\&quot;)=\&quot;UDF000UDF001\&quot;,\&quot;OK\&quot;,\&quot;Expect UDF000UDF001\&quot;)&quot;;
            cells[7, 0].Formula = &quot;=&apos;&quot; + addInFileAbs + &quot;&apos;!TEST_UDF()&quot;;
            cells[7, 1].Formula = &quot;=IF(IFERROR(A8,\&quot;Error\&quot;)=\&quot;UDF222\&quot;,\&quot;OK\&quot;,\&quot;Expect UDF222\&quot;)&quot;;
            cells[8, 0].Formula = &quot;=&apos;&quot; + addInFileAbs + &quot;&apos;!TEST_UDF()&amp;TEST_UDF1()&quot;;
            cells[8, 1].Formula = &quot;=IF(IFERROR(A9,\&quot;Error\&quot;)=\&quot;UDF222UDF001\&quot;,\&quot;OK\&quot;,\&quot;Expect UDF222UDF001\&quot;)&quot;;
            cells[6, 0].Formula = &quot;=TEST_UDF()&amp;TEST_UDF1()&quot;;
            cells[6, 1].Formula = &quot;=IF(IFERROR(A7,\&quot;Error\&quot;)=\&quot;UDF000UDF001\&quot;,\&quot;OK\&quot;,\&quot;Expect UDF000UDF001\&quot;)&quot;;
            if (ext == &quot;xls&quot;)
            {
                Util.SetHintMessage(cells[5, 1], &quot;However, for XLS only A7 can work after openning the AddIn file&quot;);
            }
            Util.SaveManCheck(wb, &quot;Formula&quot;, &quot;CELLSNET46535.&quot; + ext);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Adds addin function into the workbook

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| id | Int32 | ID of the data which contains addin functions, can be got by the first call of `RegisterAddInFunction` for the same addin file. |
| functionName | String | the addin function name |

### Return Value

URL of the addin file which contains addin functions

### Examples

```csharp
// Called: wb.Worksheets.RegisterAddInFunction(id, &amp;quot;customfunc2&amp;quot;);
private void Method_String_(Workbook wb, string[] funcs)
        {
            int id = wb.Worksheets.RegisterAddInFunction(&quot;externallink1.xlam&quot;, &quot;customfunc1&quot;, false);
            wb.Worksheets.RegisterAddInFunction(id, &quot;customfunc2&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 4; i++)
            {
                cells[i, 0].Formula = &quot;=&quot; + funcs[i];
            }
            for (int i = 1; i &lt; 5; i++)
            {
                string el = &quot;=&apos;externallink&quot; + i + &quot;.xlam&apos;!&quot;;
                for (int j = 0; j &lt; 4; j++)
                {
                    cells[j, i].Formula = el + funcs[j];
                }
            }
            cells[0, 5].Formula = &quot;&apos;[externallink1.xlam]Sheet1&apos;!$A$1&quot;;
            cells[0, 6].Formula = &quot;&apos;[externallink1.xlam]Sheet2&apos;!$A$1&quot;;
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


