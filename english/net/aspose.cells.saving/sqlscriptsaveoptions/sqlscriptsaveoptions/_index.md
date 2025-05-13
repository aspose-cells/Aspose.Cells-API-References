---
title: SqlScriptSaveOptions.SqlScriptSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions constructor. Creates options for saving sql file
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions constructor

Creates options for saving sql file.

```csharp
public SqlScriptSaveOptions()
```

### Examples

```csharp
// Called: SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
public void SqlScriptSaveOptions_Constructor()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(DateTime.Now);
    SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
    sqlSaveOptions.OperatorType = SqlScriptOperatorType.Delete;
    // sqlSaveOptions.IdName = "Id";
    //sqlSaveOptions.Separator = '\n';
    sqlSaveOptions.AddBlankLineBetweenRows = true;
    //sqlSaveOptions.CreateTable = true;
    // sqlSaveOptions.CheckAllDataForColumnType = true;
    string text = SaveAsSql(wb, sqlSaveOptions);
    Assert.IsTrue(text.IndexOf("CREATE TABLE Sheet1_2(") == -1);
    Assert.IsTrue(text.IndexOf("DELETE FROM Sheet1_2 WHERE First_name = 'Simon';") != -1);
}
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


