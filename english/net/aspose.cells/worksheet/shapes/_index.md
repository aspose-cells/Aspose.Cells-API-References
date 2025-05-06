---
title: Worksheet.Shapes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Returns all drawing shapes in this worksheet
type: docs
url: /net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Returns all drawing shapes in this worksheet.

```csharp
public ShapeCollection Shapes { get; }
```

### Examples

```csharp
// Called: foreach (Shape currentShape in currentSheet.Shapes)
[Test]
        // http://www.aspose.com/community/forums/thread/285171.aspx
        // Shape.AlternativeText blank in .XLSX
        public void Property_Shapes()
        {
            Console.WriteLine(&quot;Property_Shapes()&quot;);
            string infnXls = path + @&quot;CELLSNET-23525\ExcelSource.xls&quot;;
            string infnXlsx = path + @&quot;CELLSNET-23525\ExcelSource.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;CELLSNET-23525_out.xlsx&quot;;

            Console.WriteLine(&quot;TEST 1 - Open Excel 2000 source file &apos;{0}&apos;&quot;, infnXls);
            Workbook workbook = new Workbook(infnXls);
            Worksheet currentSheet = workbook.Worksheets[0];
            foreach (Shape currentShape in currentSheet.Shapes)
            {
                string type = currentShape.GetType().ToString();
                Console.WriteLine(&quot;Shape &apos;{0}&apos; Type=&apos;{1}&apos; Alt=&apos;{2}&apos;&quot;, currentShape.Name, type, currentShape.AlternativeText);
            }
            Console.WriteLine(&quot;Save as 2007 format: &apos;{0}&apos;&quot;, outfn);
            workbook.Save(outfn, SaveFormat.Xlsx);

            Console.WriteLine(&quot; &quot;);
            Console.WriteLine(&quot;TEST 2 - Re-open 2007 file &apos;{0}&apos; and check shapes...&apos;&quot;, outfn);
            workbook = new Workbook(outfn);
            currentSheet = workbook.Worksheets[0];
            foreach (Shape currentShape in currentSheet.Shapes)
            {
                string type = currentShape.GetType().ToString();
                Console.WriteLine(&quot;Shape &apos;{0}&apos; Type=&apos;{1}&apos; Alt=&apos;{2}&apos;&quot;, currentShape.Name, type, currentShape.AlternativeText);
            }

            Console.WriteLine(&quot; &quot;);
            Console.WriteLine(&quot;TEST 3 - Open Excel 2007 source file &apos;{0}&apos;&quot;, infnXlsx);
            workbook = new Workbook(infnXlsx);
            currentSheet = workbook.Worksheets[0];
            foreach (Shape currentShape in currentSheet.Shapes)
            {
                string type = currentShape.GetType().ToString();
                Console.WriteLine(&quot;Shape &apos;{0}&apos; Type=&apos;{1}&apos; Alt=&apos;{2}&apos;&quot;, currentShape.Name, type, currentShape.AlternativeText);
            }
        }
```

### See Also

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


