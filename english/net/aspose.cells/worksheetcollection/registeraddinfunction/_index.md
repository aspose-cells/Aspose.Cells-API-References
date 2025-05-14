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
// Called: wb.Worksheets.RegisterAddInFunction(addInFileAbs, "TEST_UDF", false);
private void WorksheetCollection_Method_RegisterAddInFunction(string ext)
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 16.0);
            string addInFileRel = "..\\..\\..\\template\\Formula\\AddIn1.xlam";
            string addInFileAbs = Path.GetFullPath(Constants.sourcePath + "Formula\\AddIn2.xlam");
            int id = wb.Worksheets.RegisterAddInFunction(addInFileRel, "TEST_UDF", false);
            wb.Worksheets.RegisterAddInFunction(id, "TEST_UDF1");
            wb.Worksheets.RegisterAddInFunction(addInFileAbs, "TEST_UDF", false);
            Util.SetHintMessage(cells[0, 0], "Before AddIn files being loaded(Macros should also be enabled), all formulas are Error values(#NAME! and error messages)");
            Util.SetHintMessage(cells[1, 0], "After loading [" + addInFileRel + "], A5:B7 should have no error");
            Util.SetHintMessage(cells[2, 0], "After loading [" + addInFileAbs + "], A8:B9 should have no error");
            cells[4, 0].Formula = "='" + addInFileRel + "'!TEST_UDF()";
            cells[4, 1].Formula = "=IF(IFERROR(A5,\"Error\")=\"UDF000\",\"OK\",\"Expect UDF000\")";
            cells[5, 0].Formula = "='" + addInFileRel + "'!TEST_UDF()&TEST_UDF1()";
            cells[5, 1].Formula = "=IF(IFERROR(A6,\"Error\")=\"UDF000UDF001\",\"OK\",\"Expect UDF000UDF001\")";
            cells[7, 0].Formula = "='" + addInFileAbs + "'!TEST_UDF()";
            cells[7, 1].Formula = "=IF(IFERROR(A8,\"Error\")=\"UDF222\",\"OK\",\"Expect UDF222\")";
            cells[8, 0].Formula = "='" + addInFileAbs + "'!TEST_UDF()&TEST_UDF1()";
            cells[8, 1].Formula = "=IF(IFERROR(A9,\"Error\")=\"UDF222UDF001\",\"OK\",\"Expect UDF222UDF001\")";
            cells[6, 0].Formula = "=TEST_UDF()&TEST_UDF1()";
            cells[6, 1].Formula = "=IF(IFERROR(A7,\"Error\")=\"UDF000UDF001\",\"OK\",\"Expect UDF000UDF001\")";
            if (ext == "xls")
            {
                Util.SetHintMessage(cells[5, 1], "However, for XLS only A7 can work after openning the AddIn file");
            }
            Util.SaveManCheck(wb, "Formula", "CELLSNET46535." + ext);
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
// Called: wb.Worksheets.RegisterAddInFunction(id, "customfunc2");
private void WorksheetCollection_Method_RegisterAddInFunction(Workbook wb, string[] funcs)
        {
            int id = wb.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            wb.Worksheets.RegisterAddInFunction(id, "customfunc2");
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 4; i++)
            {
                cells[i, 0].Formula = "=" + funcs[i];
            }
            for (int i = 1; i < 5; i++)
            {
                string el = "='externallink" + i + ".xlam'!";
                for (int j = 0; j < 4; j++)
                {
                    cells[j, i].Formula = el + funcs[j];
                }
            }
            cells[0, 5].Formula = "'[externallink1.xlam]Sheet1'!$A$1";
            cells[0, 6].Formula = "'[externallink1.xlam]Sheet2'!$A$1";
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


