---
title: SqlScriptSaveOptions.TableName
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets and sets the table name
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/tablename/
---
## SqlScriptSaveOptions.TableName property

Gets and sets the table name.

```csharp
public string TableName { get; set; }
```

### Examples

```csharp
// Called: sqlSaveOptions.TableName = "";
public void SqlScriptSaveOptions_Property_TableName()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(DateTime.Now);
    SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
    sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
    sqlSaveOptions.IdName = "";
    sqlSaveOptions.TableName = "";
    sqlSaveOptions.Separator = '\n';
    sqlSaveOptions.AddBlankLineBetweenRows = true;
    sqlSaveOptions.CreateTable = true;
    sqlSaveOptions.CheckAllDataForColumnType = true;
    string text = SaveAsSql(wb, sqlSaveOptions);
    //Assert.IsTrue(text.IndexOf("INSERT INTO Sheet1_2 (First_name,Last_name,agesdf,Column_4,tax,safs)") != -1);
    Assert.IsTrue(text.IndexOf("Id int,") == -1);
}
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


