---
title: ImageOrPrintOptions.TextCrossType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets displaying text type when the text width is larger than cell width
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/textcrosstype/
---
## ImageOrPrintOptions.TextCrossType property

Gets or sets displaying text type when the text width is larger than cell width.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Examples

```csharp
// Called: _saveOptions.TextCrossType = TextCrossType.Default;
private ImageOrPrintOptions ImageOrPrintOptions_Property_TextCrossType()
        {
            ImageOrPrintOptions _saveOptions = new ImageOrPrintOptions();
            _saveOptions.OnePagePerSheet = true;
            _saveOptions.ImageType = ImageType.Png;
            _saveOptions.TextCrossType = TextCrossType.Default;

            return _saveOptions;
        }
```

### See Also

* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


