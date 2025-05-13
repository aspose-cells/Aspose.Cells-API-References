---
title: SheetRender.ToImage
second_title: Aspose.Cells for .NET API Reference
description: SheetRender method. Render certain page to a Graphics
type: docs
url: /net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Render certain page to a Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |
| width | Single | The maximum width (in pixels) that can be occupied by the rendered page. |
| height | Single | The maximum height (in pixels) that can be occupied by the rendered page. |

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Render certain page to a Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

Render certain page to a file.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| fileName | String | filename of the output image |

### Examples

The following code outputs the first page of the first sheet to png image.

```csharp
//load the source file with images.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//set output image type.
imgOpt.ImageType = ImageType.Png;

//render the first sheet.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//output the first page of the sheet to image.
sr.ToImage(0, "output.png");
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Render certain page to a stream.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| stream | Stream | the stream of the output image |

### Examples

```csharp
// Called: renderer.ToImage(0, stream);
public void SheetRender_Method_ToImage()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    ImageOrPrintOptions options = new ImageOrPrintOptions();
    options.ImageType = ImageType.Bmp;
    options.OutputBlankPageWhenNothingToPrint = true;

    for (int i = 0; i < workbook.Worksheets.Count; i++)
    {
        if (workbook.Worksheets[i].IsVisible)
        {
            using (Stream stream = File.Open(Path.Combine(Constants.destPath, "{i}.png"),
                FileMode.OpenOrCreate, FileAccess.ReadWrite))
            {
                SheetRender renderer = new SheetRender(workbook.Worksheets[i], options);
                renderer.ToImage(0, stream);
            }
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Render certain page to a Bitmap object.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |

### Return Value

the bitmap object of the page

### Examples

```csharp
// Called: var image = sh1.ToImage(0);
        public void SheetRender_Method_ToImage()
        {
            var workbook = new Workbook();
            workbook.Worksheets[0].PageSetup.PrintArea = "A1:A1";
            workbook.Worksheets[0].Cells["A1"].PutValue("");
            var test = workbook.Worksheets[0].Cells["A1"].Characters(0, 0);


            var opt = new ImageOrPrintOptions
            {
                PrintingPage = PrintingPageType.IgnoreBlank,
                //ImageFormat = ImageFormat.Png,
                ImageType = ImageType.Png,
                OnePagePerSheet = true,
                OnlyArea = true
            };
            var sh1 = new SheetRender(workbook.Worksheets[0], opt);
#if !NETCOREAPP2_0
            var image = sh1.ToImage(0);
#else
            sh1.ToImage(0, Constants.destPath + "example.png");
#endif
        }
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


