---
title: Style.IsDateTime
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates whether the number format is a date format
type: docs
url: /net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Indicates whether the number format is a date format.

```csharp
public bool IsDateTime { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(style.IsDateTime,true);
public void Style_Property_IsDateTime()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A1"].PutValue(1230);
    Style style = cells["A1"].GetStyle();
    style.Number = 15;
    Assert.AreEqual(style.IsDateTime,true);
    style.Custom = "yyyy-mm-dd";
      Assert.AreEqual(style.IsDateTime,true);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


