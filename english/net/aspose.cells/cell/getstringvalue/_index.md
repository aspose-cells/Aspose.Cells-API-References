---
title: Cell.GetStringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the string value by specific formatted strategy
type: docs
url: /net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Gets the string value by specific formatted strategy.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | The formatted strategy. |

### Examples

```csharp
// Called: string str = cells["A1"].GetStringValue(CellValueFormatStrategy.None);
[Test]
        public void Method_CellValueFormatStrategy_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            string str = cells["A1"].GetStringValue(CellValueFormatStrategy.None);
        }
```

### See Also

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


