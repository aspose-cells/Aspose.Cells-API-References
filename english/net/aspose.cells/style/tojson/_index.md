---
title: Style.ToJson
second_title: Aspose.Cells for .NET API Reference
description: Style method. Convert Style to JSON struct data
type: docs
url: /net/aspose.cells/style/tojson/
---
## Style.ToJson method

Convert [`Style`](../) to JSON struct data.

```csharp
public string ToJson()
```

### Examples

```csharp
// Called: string json = style.ToJson();
[Test]
        public void Method_ToJson()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET52627.xlsx");
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells["B4"].GetStyle();
            string json = style.ToJson();
            Assert.IsTrue(json.IndexOf("\"backgroundColor\" : \"#FFFFFF00\"") != -1);
            Cell cell = cells["B6"];
            json = cell.ToJson();
            Assert.IsTrue(json.IndexOf("\"formula\" : \"=A1\"") != -1);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


