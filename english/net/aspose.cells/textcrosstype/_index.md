---
title: Enum TextCrossType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.TextCrossType enum. Enumerates displaying text type when the text width is larger than cell width
type: docs
url: /net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Enumerates displaying text type when the text width is larger than cell width.

```csharp
public enum TextCrossType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Default | `1` | Display text like in Microsoft Excel. |
| CrossKeep | `2` | Display all the text by crossing other cells and keep text of crossed cells. |
| CrossOverride | `3` | Display all the text by crossing other cells and override text of crossed cells. |
| StrictInCell | `4` | Only display the text within the width of cell. |

### Examples

```csharp
// Called: _saveOptions.TextCrossType = TextCrossType.Default;
private ImageOrPrintOptions Cells_Type_TextCrossType()
        {
            ImageOrPrintOptions _saveOptions = new ImageOrPrintOptions();
            _saveOptions.OnePagePerSheet = true;
            _saveOptions.ImageType = ImageType.Png;
            _saveOptions.TextCrossType = TextCrossType.Default;

            return _saveOptions;
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


