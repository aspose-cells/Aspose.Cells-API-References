---
title: MsoLineFormat.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Indicates whether the object is visible
type: docs
url: /net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Indicates whether the object is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(currentSheet.Shapes[0].LineFormat.IsVisible);
// Aspose.Cells addes border to Bitmaps when saving to 2007 formats
// http://www.aspose.com/community/forums/thread/293742.aspx
public void MsoLineFormat_Property_IsVisible()
{
    Console.WriteLine("MsoLineFormat_Property_IsVisible()");
    string infn = path + @"BitmapBorder\ExcelSource.xlsx";
    string outfn = Constants.destPath + @"ExcelSource_output.xlsx";
    string infnXlsm = path + @"BitmapBorder\ExcelSource.xlsm";
    string outfnXlsm = Constants.destPath + @"ExcelSource_output.xlsm";

    Console.WriteLine("TEST 1 - Open Excel source file '{0}'", infn);
    Workbook workbook = new Workbook(infn);
    Worksheet currentSheet = workbook.Worksheets[0];
    Assert.IsFalse(currentSheet.Shapes[0].LineFormat.IsVisible);
    Assert.IsTrue(currentSheet.Shapes[1].LineFormat.IsVisible);
    Console.WriteLine("Save file to: '{0}'", outfn);
    workbook.Save(outfn, SaveFormat.Xlsx);

    workbook = null;

    Console.WriteLine("TEST 2 - Open Excel source file '{0}'", infnXlsm);
    workbook = new Workbook(infnXlsm);
    currentSheet = workbook.Worksheets[0];
    Assert.IsFalse(currentSheet.Shapes[0].LineFormat.IsVisible);
    Assert.IsTrue(currentSheet.Shapes[1].LineFormat.IsVisible);
    Console.WriteLine("Save file to: '{0}'", outfnXlsm);
    workbook.Save(outfnXlsm, SaveFormat.Xlsm);
}
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


