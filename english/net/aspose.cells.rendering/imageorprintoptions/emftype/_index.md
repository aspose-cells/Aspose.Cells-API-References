---
title: ImageOrPrintOptions.EmfType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Examples

```csharp
// Called: options.EmfType = System.Drawing.Imaging.EmfType.EmfOnly;
public void ImageOrPrintOptions_Property_EmfType()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    sheet.Cells["A1"].PutValue("Test output Emf Type");

    var options = new ImageOrPrintOptions();
    options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;
    options.OnlyArea = true;

    MemoryStream ms = new MemoryStream();
    SheetRender sr1 = new SheetRender(sheet, options);
    sr1.ToImage(0, ms);
    int emfPlusDualLength = ms.ToArray().Length;

    ms = new MemoryStream();
    options.EmfType = System.Drawing.Imaging.EmfType.EmfOnly;
    SheetRender sr2 = new SheetRender(sheet, options);
    sr2.ToImage(0, ms);
    int emfOnlyLength = ms.ToArray().Length;

    Assert.IsTrue(emfOnlyLength < emfPlusDualLength);
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


