---
title: SqlScriptSaveOptions.Separator
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets and sets character separator of sql script
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/separator/
---
## SqlScriptSaveOptions.Separator property

Gets and sets character separator of sql script.

```csharp
public char Separator { get; set; }
```

### Remarks

Only can be ' ' or '\n'. If the

### Examples

```csharp
// Called: sqlSaveOptions.Separator = '\n';
[Test]
        public void Property_Separator()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet49680.xlsx");
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


