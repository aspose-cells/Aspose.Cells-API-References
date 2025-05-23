---
title: Enum TargetModeType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.TargetModeType enum. Represents the type of target mode
type: docs
url: /net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Represents the type of target mode.

```csharp
public enum TargetModeType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| External | `0` | External link |
| FilePath | `1` | Local and full paths to files or folders. |
| Email | `2` | Email. |
| CellReference | `3` | Link on cell or named range. |

### Examples

```csharp
// Called: Assert.AreEqual(TargetModeType.External, links[0].LinkType);
public void Cells_Type_TargetModeType()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "www.aspose.com");
    Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("A1");
    Hyperlink[] links = range.Hyperlinks;
    Assert.AreEqual(TargetModeType.External, links[0].LinkType);
    if(links.Length != 0)
    {
        links[0].Delete();
    }
    Assert.AreEqual(0, workbook.Worksheets[0].Hyperlinks.Count); 
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


