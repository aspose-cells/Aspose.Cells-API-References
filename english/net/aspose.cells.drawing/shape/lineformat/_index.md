---
title: Shape.LineFormat
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Returns a MsoLineFormat object that contains line formatting properties for the specified shape
type: docs
url: /net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Returns a MsoLineFormat object that contains line formatting properties for the specified shape.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Assert.IsTrue(currentSheet.Shapes[1].LineFormat.IsVisible);
[Test]
        // Aspose.Cells addes border to Bitmaps when saving to 2007 formats
        // http://www.aspose.com/community/forums/thread/293742.aspx
        public void Property_LineFormat()
        {
            Console.WriteLine(&quot;Property_LineFormat()&quot;);
            string infn = path + @&quot;BitmapBorder\ExcelSource.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;ExcelSource_output.xlsx&quot;;
            string infnXlsm = path + @&quot;BitmapBorder\ExcelSource.xlsm&quot;;
            string outfnXlsm = Constants.destPath + @&quot;ExcelSource_output.xlsm&quot;;

            Console.WriteLine(&quot;TEST 1 - Open Excel source file &apos;{0}&apos;&quot;, infn);
            Workbook workbook = new Workbook(infn);
            Worksheet currentSheet = workbook.Worksheets[0];
            Assert.IsFalse(currentSheet.Shapes[0].LineFormat.IsVisible);
            Assert.IsTrue(currentSheet.Shapes[1].LineFormat.IsVisible);
            Console.WriteLine(&quot;Save file to: &apos;{0}&apos;&quot;, outfn);
            workbook.Save(outfn, SaveFormat.Xlsx);

            workbook = null;

            Console.WriteLine(&quot;TEST 2 - Open Excel source file &apos;{0}&apos;&quot;, infnXlsm);
            workbook = new Workbook(infnXlsm);
            currentSheet = workbook.Worksheets[0];
            Assert.IsFalse(currentSheet.Shapes[0].LineFormat.IsVisible);
            Assert.IsTrue(currentSheet.Shapes[1].LineFormat.IsVisible);
            Console.WriteLine(&quot;Save file to: &apos;{0}&apos;&quot;, outfnXlsm);
            workbook.Save(outfnXlsm, SaveFormat.Xlsm);
        }
```

### See Also

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


