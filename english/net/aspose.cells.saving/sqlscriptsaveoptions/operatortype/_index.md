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
// Called: sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
[Test]
        public void Property_OperatorType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet49680.xlsx&quot;);
            Console.WriteLine(DateTime.Now);
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
             sqlSaveOptions.IdName = &quot;Id&quot;;
            sqlSaveOptions.TableName = &quot;&quot;;
            sqlSaveOptions.Separator = &apos;\n&apos;;
            sqlSaveOptions.AddBlankLineBetweenRows = true;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true;
            string text = SaveAsSql(wb, sqlSaveOptions);
            //Assert.IsTrue(text.IndexOf(&quot;INSERT INTO Sheet1_2 (First_name,Last_name,agesdf,Column_4,tax,safs)&quot;) != -1);
            Assert.IsTrue(text.IndexOf(&quot;Id int,&quot;) != -1);
        }
```

### See Also

* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


