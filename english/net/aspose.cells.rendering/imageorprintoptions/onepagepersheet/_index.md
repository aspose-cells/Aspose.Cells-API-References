---
title: ImageOrPrintOptions.OnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. If OnePagePerSheet is true  all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: _saveOptions.OnePagePerSheet = true;
private ImageOrPrintOptions ImageOrPrintOptions_Property_OnePagePerSheet()
        {
            ImageOrPrintOptions _saveOptions = new ImageOrPrintOptions();
            _saveOptions.OnePagePerSheet = true;
            _saveOptions.ImageType = ImageType.Png;
            _saveOptions.TextCrossType = TextCrossType.Default;

            return _saveOptions;
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


