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
[Test]
        public void Property_AddBlankLineBetweenRows()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet49680.xlsx&quot;);
            Console.WriteLine(DateTime.Now);
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Delete;
            // sqlSaveOptions.IdName = &quot;Id&quot;;
            sqlSaveOptions.Separator = &apos;\n&apos;;
            sqlSaveOptions.AddBlankLineBetweenRows = true;
            sqlSaveOptions.CreateTable = true;
            string text = SaveAsSql(wb, sqlSaveOptions);
            Assert.IsTrue(text.IndexOf(&quot;CREATE TABLE Sheet1_2(&quot;) != -1);
            Assert.IsTrue(text.IndexOf(&quot;First_name = &apos;Simon&apos;;&quot;) != -1);
            Assert.IsTrue(text.IndexOf(&quot;tax DOUBLE,&quot;) != -1);
        }
```

### See Also

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


