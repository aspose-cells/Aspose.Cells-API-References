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
        public void Method_Stream_()//CELLSNETCORE-41
        {
            string path = Constants.TemplatePath + &quot;NetCoreTests/CELLSNET46962/&quot;;
            string name = &quot;02_sheet_pwd_xlsx&quot;;
            var filePath = path + name + &quot;.xlsx&quot;;
            var loadOptions = new Aspose.Cells.LoadOptions();
            loadOptions.Password = &quot;1234567890&quot;;
            using (Aspose.Cells.Workbook document = filePath.Contains(&quot;pwd&quot;) ? new Workbook(filePath, loadOptions) : new Workbook(filePath))
            {
                int sheetCount = document.Worksheets.Count;
                for (var sheetNum = 0; sheetNum &lt; sheetCount; ++sheetNum)
                {
                    Aspose.Cells.Worksheet sheet = document.Worksheets[sheetNum];
                    Aspose.Cells.Rendering.ImageOrPrintOptions imgOptions =
                        new Aspose.Cells.Rendering.ImageOrPrintOptions();
                    imgOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    imgOptions.OnePagePerSheet = true;
                    Aspose.Cells.Rendering.SheetRender sr = new Aspose.Cells.Rendering.SheetRender(sheet, imgOptions);
                    //One worksheet may be printed as mutiple pages
                    //This &quot;pageCount&quot; means how many pages will this worksheet be printed
                    int pageCount = sr.PageCount;
                    for (var pageNum = 0; pageNum &lt; pageCount; ++pageNum)
                    {
                        using (Stream stream = new MemoryStream())
                        {
                            stream.Position = 0;
                            sr.ToImage(pageNum, stream);
                            string s1 = String.Format(&quot;Sheet{0}_Page{1}&quot;, sheetNum, pageNum);
                            if (stream.Length == 0)
                            {
                                //Console.WriteLine($&quot;File ({pages}-pages): {System.IO.Path.GetFileName(filePath)} - page {pageNumber} - NO IMAGE&quot;);
                            }
                            else
                            {
                                //Console.WriteLine($&quot;File ({pages}-pages): {System.IO.Path.GetFileName(filePath)} - page {pageNumber} - GOOD&quot;);

                                StreamWriter sw = new StreamWriter(destPathNetCore + name + s1 + &quot;.png&quot;);
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
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;21010_2003.xls&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = ImageType.Jpeg;
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            Bitmap bitmap = sheetRender.ToImage(0);
            bitmap.Save(Constants.destPath + &quot;21010_2003.jpg&quot;, ImageFormat.Jpeg);
        }
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


