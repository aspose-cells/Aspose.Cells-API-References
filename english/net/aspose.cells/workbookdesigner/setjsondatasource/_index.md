---
title: WorkbookDesigner.SetJsonDataSource
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. 
type: docs
url: /net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

```csharp
public void SetJsonDataSource(string variable, string data)
```

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String |  |
| data | String |  |

### Examples

```csharp
// Called: designer.SetJsonDataSource(&amp;quot;ds&amp;quot;, data);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA45705_2.xlsx&quot;);
            String data = &quot;{\n&quot; + &quot;    \&quot;array\&quot;: [\n&quot; + &quot;        \&quot;English\&quot;,\n&quot; + &quot;        \&quot;Arabic\&quot;,\n&quot;
                  + &quot;        \&quot;Hindi\&quot;,\n&quot; + &quot;        \&quot;Urdu\&quot;,\n&quot; + &quot;        \&quot;French\&quot;\n&quot; + &quot;    ],\n&quot;
                  + &quot;    \&quot;var\&quot;: \&quot;This is a sentence using one place holder\&quot;,\n&quot; + &quot;\&quot;arrObj\&quot;: [\n&quot; + &quot;    {\n&quot;
                  + &quot;        \&quot;name\&quot;: \&quot;John Doe\&quot;,\n&quot; + &quot;        \&quot;age\&quot;: \&quot;27\&quot;\n&quot; + &quot;    },\n&quot; + &quot;    {\n&quot;
                  + &quot;        \&quot;name\&quot;: \&quot;Jane Doe\&quot;,\n&quot; + &quot;        \&quot;age\&quot;: \&quot;27\&quot;\n&quot; + &quot;    }\n&quot; + &quot;]&quot; + &quot;}&quot;;

            WorkbookDesigner designer = new WorkbookDesigner(wb);
            designer.SetJsonDataSource(&quot;ds&quot;, data);
            designer.LineByLine = false;

            designer.Process();
            wb.Save(Constants.destPath + &quot;CELLSJAVA45705_2.xlsx&quot;);
            Assert.AreEqual(&quot;Arabic&quot;, wb.Worksheets[0].Cells[&quot;A9&quot;].StringValue);
            Assert.AreEqual(&quot;27&quot;, wb.Worksheets[0].Cells[&quot;B3&quot;].StringValue);

        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


