---
title: CellsHelper.DPI
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets the DPI of the machine
type: docs
url: /net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Gets the DPI of the machine.

```csharp
public static double DPI { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(CellsHelper.DPI);
public void CellsHelper_Property_DPI()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42018/";
    Console.WriteLine(CellsHelper.DPI);

    Workbook wb = new Workbook(filePath + "bg2_border.xlsx");
    wb.Save(Constants.destPath + "example.html");
    wb =new Workbook(Constants.destPath + "example.html");
    Assert.AreEqual(2, wb.Worksheets[0].Shapes.Count);
           
    HtmlSaveOptions o = new HtmlSaveOptions();
    ImageOrPrintOptions imgOptions = o.ImageOptions;
    //imgOptions.SaveFormat = SaveFormat.Svg;
    //imgOptions.ImageFormat = ImageFormat.Icon;
    imgOptions.ImageType = ImageType.Emf;
    wb.Save(Constants.destPath + "example.html");
    wb = new Workbook(Constants.destPath + "example.html");
    Assert.AreEqual(2, wb.Worksheets[0].Shapes.Count);
}
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


