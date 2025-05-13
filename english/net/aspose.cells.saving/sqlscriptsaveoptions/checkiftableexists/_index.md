---
title: SqlScriptSaveOptions.CheckIfTableExists
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Check if the table name exists before creating
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/
---
## SqlScriptSaveOptions.CheckIfTableExists property

Check if the table name exists before creating

```csharp
public bool CheckIfTableExists { get; set; }
```

### Examples

```csharp
// Called: sqlSaveOptions.CheckIfTableExists = true;
public void SqlScriptSaveOptions_Property_CheckIfTableExists()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(DateTime.Now);
    SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
    sqlSaveOptions.OperatorType = SqlScriptOperatorType.Delete;
    // sqlSaveOptions.IdName = "Id";
    //sqlSaveOptions.Separator = '\n';
    sqlSaveOptions.AddBlankLineBetweenRows = true;
    sqlSaveOptions.CreateTable = true;
    sqlSaveOptions.CheckIfTableExists = true;
    // sqlSaveOptions.CheckAllDataForColumnType = true;
    string text = SaveAsSql(wb, sqlSaveOptions);
    Assert.IsTrue(text.IndexOf("CREATE TABLE IF NOT EXISTS Sheet1_2") != -1);
    Assert.IsTrue(text.IndexOf("DELETE FROM Sheet1_2 WHERE First_name = 'Simon';") != -1);
}
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


