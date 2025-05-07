---
title: ScrollBar.IsHorizontal
second_title: Aspose.Cells for .NET API Reference
description: ScrollBar property. Indicates whether this is a horizontal scroll bar
type: docs
url: /net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Indicates whether this is a horizontal scroll bar.

```csharp
public bool IsHorizontal { get; set; }
```

### Examples

```csharp
// Called: if (!bar1.IsHorizontal || !bar2.IsHorizontal)
[Test]
        // http://www.aspose.com/community/forums/thread/255449.aspx
        public void Property_IsHorizontal()
        {
            Console.WriteLine("Property_IsHorizontal()");
            string infn = path + "Test_HorizontalScrollBar.xlsx";
            string outfn = Constants.destPath + "Test_HorizontalScrollBar_out.xlsx";

            Workbook book = new Workbook(infn);
            ShapeCollection shapes = book.Worksheets[0].Shapes;
            ScrollBar bar1 = null;
            foreach (Shape s in shapes)
            {
                if (s.MsoDrawingType == MsoDrawingType.ScrollBar)
                {
                    bar1 = (ScrollBar)s;
                    break;
                }
            }

            book.Save(outfn);

            Workbook book2 = new Workbook(outfn);
            shapes = book2.Worksheets[0].Shapes;
            ScrollBar bar2 = null;
            foreach (Shape s in shapes)
            {
                if (s.MsoDrawingType == MsoDrawingType.ScrollBar)
                {
                    bar2 = (ScrollBar)s;
                    break;
                }
            }

            if (!bar1.IsHorizontal || !bar2.IsHorizontal)
                throw new Exception("Property_IsHorizontal() failed!");
        }
```

### See Also

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


