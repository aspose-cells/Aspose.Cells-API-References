---
title: ImageOrPrintOptions.SetDesiredSize
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions method. Sets desired width and height of image
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Sets desired width and height of image.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Int32 | desired width in pixels |
| desiredHeight | Int32 | desired height in pixels |

### Remarks

NOTE: This member is now obsolete. Instead, please use `SetDesiredSize` by setting param keepAspectRatio to false. This property will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: options.SetDesiredSize(2560, 1440);
[Test]
        public void Method_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA43139_";

            Workbook workbook = new Workbook(filePath + "template.xlsx");

            String filename = "template";
            string startPoint = "B1";
            string endPoint = "P14";
            int sheetIndex = 1;
            String picName = filename + "_" + startPoint + "_" + endPoint + ".jpg";  // png            
            string resultPath = CreateFolder(filePath) + picName;
            Worksheet worksheet = workbook.Worksheets[sheetIndex];

            String printArea = startPoint + ":" + endPoint;
            Console.WriteLine("area: " + printArea);

            worksheet.PageSetup.PrintArea = printArea;
            worksheet.PageSetup.LeftMargin = 1;
            worksheet.PageSetup.RightMargin = 1;
            worksheet.PageSetup.TopMargin = 1;
            worksheet.PageSetup.BottomMargin = 1;

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(2560, 1440);
            options.ImageType = ImageType.Jpeg;
            // options.setCellAutoFit(true);
            //CellsHelper.FontDir = @"C:\Windows\Fonts";

            DateTime now = DateTime.Now;
            workbook.Worksheets.RefreshPivotTables();
            Console.WriteLine(DateTime.Now.Subtract(now).ToString());
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet s = workbook.Worksheets[i];
                ChartCollection charts = s.Charts;
                for (int j = 0; j < charts.Count; j++)
                {
                    Chart chart = s.Charts[j];

                    s.Charts[j].RefreshPivotData();
                }
            }
            workbook.CalculateFormula();

            SheetRender sheetRender = new SheetRender(worksheet, options);
            Console.WriteLine("size -> " + sheetRender.PageCount);
            for (int i = 0; i < sheetRender.PageCount; i++)
            {
                sheetRender.ToImage(i, resultPath);
            }

            workbook.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Sets desired width and height of image.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Int32 | desired width in pixels |
| desiredHeight | Int32 | desired height in pixels |
| keepAspectRatio | Boolean | whether to keep aspect ratio of origin image |

### Remarks

The width and height of the output image in pixels will be only based on the set desired width and height.

The [`HorizontalResolution`](../horizontalresolution/) and [`VerticalResolution`](../verticalresolution/) will not effect the width and height of the output image in this case.

### Examples

```csharp
// Called: options.SetDesiredSize(shape.Width, shape.Height, false);
[Test]
        public void Method_Boolean_()
        {
            string xlFile = Constants.TemplatePath + "CELLSJAVA-43064.xlsx";
            string shapeName = "Chart 1";

            Workbook wb = new Workbook(xlFile);
            Shape shape = wb.Worksheets[0].Shapes[shapeName];

            // Convert the Shape to SVG
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Svg;
            options.SetDesiredSize(shape.Width, shape.Height, false);
            options.IsOptimized = true;

            MemoryStream ms = new MemoryStream();
            shape.ToImage(ms, options);

            //less than 16k
            Assert.Less(ms.Length, 16 * 1024);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


