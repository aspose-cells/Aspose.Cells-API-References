---
title: SqlScriptSaveOptions.CreateTable
second_title: Aspose.Cells for .NET API Reference
description: SqlScriptSaveOptions property. Indicates whether exporting sql of creating table
type: docs
url: /net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

Indicates whether exporting sql of creating table.

```csharp
public bool CreateTable { get; set; }
```

### Examples

```csharp
// Called: sqlSaveOptions.CreateTable = true;
[Test]
        public void Property_CreateTable()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet49680.xlsx");
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

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


