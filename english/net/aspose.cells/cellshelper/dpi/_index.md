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
[Test]
        public void Property_DPI()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42018/&quot;;
            Console.WriteLine(CellsHelper.DPI);

            Workbook wb = new Workbook(filePath + &quot;bg2_border.xlsx&quot;);
            wb.Save(Constants.destPath + &quot;JAVA42018.html&quot;);
            wb =new Workbook(Constants.destPath + &quot;JAVA42018.html&quot;);
            Assert.AreEqual(2, wb.Worksheets[0].Shapes.Count);
           
            HtmlSaveOptions o = new HtmlSaveOptions();
            ImageOrPrintOptions imgOptions = o.ImageOptions;
            //imgOptions.SaveFormat = SaveFormat.Svg;
            //imgOptions.ImageFormat = ImageFormat.Icon;
            imgOptions.ImageType = ImageType.Emf;
            wb.Save(Constants.destPath + &quot;JAVA42018_1.html&quot;);
            wb = new Workbook(Constants.destPath + &quot;JAVA42018_1.html&quot;);
            Assert.AreEqual(2, wb.Worksheets[0].Shapes.Count);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


