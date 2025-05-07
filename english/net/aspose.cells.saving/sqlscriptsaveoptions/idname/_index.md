---
title: SqlScriptSaveOptions.IdName
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Gets and sets the name of id column
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Gets and sets the name of id column.

```csharp
public string IdName { get; set; }
```

### Remarks

If this property is set , a column will be inserted with automatical increment int value.

### Examples

```csharp
// Called: sqlSaveOptions.IdName = "Id";
[Test]
        public void Property_IdName()
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


