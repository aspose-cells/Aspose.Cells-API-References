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
// Called: sr.ToImage(pageNum, stream);
[Test]
        public void Method_Stream_()
        {
            string path = Constants.TemplatePath + "NetCoreTests/CELLSNET46962/";
            var filePath = path + "02_sheet_xlsx.xlsx";
            var loadOptions = new Aspose.Cells.LoadOptions();
            loadOptions.Password = "1234567890";
            using (Aspose.Cells.Workbook document = filePath.Contains("pwd") ? new Workbook(filePath, loadOptions) : new Workbook(filePath))
            {
                int sheetCount = document.Worksheets.Count;
                for (var sheetNumber = 0; sheetNumber < sheetCount; ++sheetNumber)
                {
                    Aspose.Cells.Worksheet sheet = document.Worksheets[sheetNumber];
                    Aspose.Cells.Rendering.ImageOrPrintOptions imgOptions = new Aspose.Cells.Rendering.ImageOrPrintOptions()
                    {
                        ImageType = Aspose.Cells.Drawing.ImageType.Png,
                        OnePagePerSheet = true
                    };
                    Aspose.Cells.Rendering.SheetRender sr = new Aspose.Cells.Rendering.SheetRender(sheet, imgOptions);
                    int pageCount = sr.PageCount;
                    for (var pageNum = 0; pageNum < pageCount; ++pageNum)
                    {
                        using (Stream stream = new MemoryStream())
                        {
                            stream.Position = 0;
                            //var bmp = sr.ToImage(pageNum);
                            //bmp.Save(stream, System.Drawing.Imaging.ImageFormat.Jpeg);
                            sr.ToImage(pageNum, stream);
                            if (stream.Length == 0)
                            {
                                Console.WriteLine($"File ({sheetCount}-pages): {System.IO.Path.GetFileName(filePath)} - page {pageNum} - NO IMAGE");
                            }
                            else
                            {
                                //var bmp = (Bitmap)Bitmap.FromStream(stream);
                                string s1 = String.Format("Sheet{0}_Page{1}", sheetNumber, pageNum);
                                Console.WriteLine($"File ({sheetCount}-pages): {System.IO.Path.GetFileName(filePath)} - page {pageNum} - GOOD");
                                StreamWriter sw = new StreamWriter(destPathNetCore + "02_sheet_xlsx_" + s1 + ".png");
                                stream.CopyTo(sw.BaseStream);
                                sw.Flush();
                                sw.Close();
                            }
                        }
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
// Called: Bitmap bitmap = sheetRender.ToImage(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_162682.xls");
            Worksheet sheet = workbook.Worksheets[0];
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = ImageType.Jpeg;
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            Bitmap bitmap = sheetRender.ToImage(0);
            bitmap.Save(Constants.destPath + "Test_162682.jpg", ImageFormat.Jpeg);
        }
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


