---
title: Cell.ToJson
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Convert Cell to JSON struct data
type: docs
url: /net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Convert [`Cell`](../) to JSON struct data.

```csharp
public string ToJson()
```

### Examples

```csharp
// Called: json = cell.ToJson();
[Test]
        public void Method_ToJson()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET52627.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[&quot;B4&quot;].GetStyle();
            string json = style.ToJson();
            Assert.IsTrue(json.IndexOf(&quot;\&quot;backgroundColor\&quot; : \&quot;#FFFFFF00\&quot;&quot;) != -1);
            Cell cell = cells[&quot;B6&quot;];
            json = cell.ToJson();
            Assert.IsTrue(json.IndexOf(&quot;\&quot;formula\&quot; : \&quot;=A1\&quot;&quot;) != -1);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


