---
title: SqlScriptSaveOptions.CheckAllDataForColumnType
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Check all data to find columns data type
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Check all data to find columns' data type.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Remarks

The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

### Examples

```csharp
// Called: sqlSaveOptions.CheckAllDataForColumnType = true;
public void SqlScriptSaveOptions_Property_CheckAllDataForColumnType()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(DateTime.Now);
    SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
    sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
    // sqlSaveOptions.IdName = "Id";
          
    sqlSaveOptions.Separator = '\n';
    sqlSaveOptions.AddBlankLineBetweenRows = true;
    sqlSaveOptions.CreateTable = true;
    sqlSaveOptions.CheckAllDataForColumnType = true;
    string text = SaveAsSql(wb, sqlSaveOptions);
    Assert.IsTrue(text.IndexOf("INSERT INTO Sheet1_2 (First_name,Last_name,age,Column_4,tax,safs)") != -1);
    Assert.IsTrue(text.IndexOf("tax VARCHAR(10),") != -1);
}
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


