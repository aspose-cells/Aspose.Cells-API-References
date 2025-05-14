---
title: SqlScriptSaveOptions.AddBlankLineBetweenRows
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Insert blank line between each data
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/
---
## SqlScriptSaveOptions.AddBlankLineBetweenRows property

Insert blank line between each data.

```csharp
public bool AddBlankLineBetweenRows { get; set; }
```

### Remarks

If [`Separator`](../separator/) is '\n' , it's better to set this property as true to increase readability.

### Examples

```csharp
// Called: sqlSaveOptions.AddBlankLineBetweenRows = true;
public void SqlScriptSaveOptions_Property_AddBlankLineBetweenRows()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(DateTime.Now);
    SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
    sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
     sqlSaveOptions.IdName = "Id";
    sqlSaveOptions.TableName = "";
    sqlSaveOptions.Separator = '\n';
    sqlSaveOptions.AddBlankLineBetweenRows = true;
    sqlSaveOptions.CreateTable = true;
    sqlSaveOptions.CheckAllDataForColumnType = true;
    string text = SaveAsSql(wb, sqlSaveOptions);
    //Assert.IsTrue(text.IndexOf("INSERT INTO Sheet1_2 (First_name,Last_name,agesdf,Column_4,tax,safs)") != -1);
    Assert.IsTrue(text.IndexOf("Id int,") != -1);
}
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


