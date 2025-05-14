---
title: PasteOptions.IgnoreLinksToOriginalFile
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. Ingore links to the original file
type: docs
url: /net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ingore links to the original file.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Examples

```csharp
// Called: pasteOptions.IgnoreLinksToOriginalFile = true;
public void PasteOptions_Property_IgnoreLinksToOriginalFile()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet src = workbook.Worksheets[0];
    var srcRange = src.Cells.CreateRange("A1:F3");
           
    int index = workbook.Worksheets.Add();
    Worksheet dst = workbook.Worksheets[index];
    Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:F3");
    ;

    PasteOptions pasteOptions = new PasteOptions();
    pasteOptions.PasteType = PasteType.All;
    pasteOptions.IgnoreLinksToOriginalFile = true;
    dstRange.Copy(srcRange, pasteOptions);
    ListObject table = workbook.Worksheets[1].ListObjects[0];
   ListColumn lo = table.ListColumns[table.ListColumns.Count - 1];
    Assert.AreEqual("=Table2[[#Headers],[Discount]]", lo.Formula);
    //CELLSNET-52834
    Assert.AreEqual("=Table2[[#Headers],[Discount]]", dst.Cells["F2"].Formula);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


