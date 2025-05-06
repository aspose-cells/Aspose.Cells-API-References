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
[Test]
        public void SqlScriptSaveOptions_Constructor()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet49680.xlsx&quot;);
            Console.WriteLine(DateTime.Now);
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Delete;
            // sqlSaveOptions.IdName = &quot;Id&quot;;
            //sqlSaveOptions.Separator = &apos;\n&apos;;
            sqlSaveOptions.AddBlankLineBetweenRows = true;
            //sqlSaveOptions.CreateTable = true;
            // sqlSaveOptions.CheckAllDataForColumnType = true;
            string text = SaveAsSql(wb, sqlSaveOptions);
            Assert.IsTrue(text.IndexOf(&quot;CREATE TABLE Sheet1_2(&quot;) == -1);
            Assert.IsTrue(text.IndexOf(&quot;DELETE FROM Sheet1_2 WHERE First_name = &apos;Simon&apos;;&quot;) != -1);
        }
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


