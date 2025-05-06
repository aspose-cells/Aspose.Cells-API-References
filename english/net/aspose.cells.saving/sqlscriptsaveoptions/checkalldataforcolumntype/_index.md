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
[Test]
        public void Property_CheckAllDataForColumnType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet49680.xlsx&quot;);
            Console.WriteLine(DateTime.Now);
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.IdName = &quot;&quot;;
            sqlSaveOptions.TableName = &quot;&quot;;
            sqlSaveOptions.Separator = &apos;\n&apos;;
            sqlSaveOptions.AddBlankLineBetweenRows = true;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true;
            string text = SaveAsSql(wb, sqlSaveOptions);
            //Assert.IsTrue(text.IndexOf(&quot;INSERT INTO Sheet1_2 (First_name,Last_name,agesdf,Column_4,tax,safs)&quot;) != -1);
            Assert.IsTrue(text.IndexOf(&quot;Id int,&quot;) == -1);
        }
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


