---
title: SqlScriptSaveOptions.OperatorType
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets and sets the operator type of sql
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/operatortype/
---
## SqlScriptSaveOptions.OperatorType property

Gets and sets the operator type of sql.

```csharp
public SqlScriptOperatorType OperatorType { get; set; }
```

### Examples

```csharp
// Called: sqlSaveOptions.OperatorType = SqlScriptOperatorType.Delete;
public void SqlScriptSaveOptions_Property_OperatorType()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(DateTime.Now);
    SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
    sqlSaveOptions.OperatorType = SqlScriptOperatorType.Delete;
    // sqlSaveOptions.IdName = "Id";
    sqlSaveOptions.Separator = '\n';
    sqlSaveOptions.AddBlankLineBetweenRows = true;
    sqlSaveOptions.CreateTable = true;
    string text = SaveAsSql(wb, sqlSaveOptions);
    Assert.IsTrue(text.IndexOf("CREATE TABLE Sheet1_2(") != -1);
    Assert.IsTrue(text.IndexOf("First_name = 'Simon';") != -1);
    Assert.IsTrue(text.IndexOf("tax DOUBLE,") != -1);
}
```

### See Also

* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


