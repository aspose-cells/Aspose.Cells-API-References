---
title: Font.Name
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the name of the Font
type: docs
url: /net/aspose.cells/font/name/
---
## Font.Name property

Gets or sets the name of the [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Examples

```csharp
// Called: style.Font.Name = &amp;quot;Tahoma&amp;quot;;
[Test]
        // http://www.aspose.com/community/forums/thread/278316/not-able-to-set-displayrsquare-datalabel-position-in-scatter-chart.aspx
        // Not able to set DisplayRSquare datalabel position in Scatter Chart
        public void Property_Name()
        {
            Console.WriteLine(&quot;Property_Name()&quot;);
            string outfnXlsx = Constants.destPath + &quot;ScatterConnected.xlsx&quot;;
            string outfnXls = Constants.destPath + &quot;ScatterConnected.xls&quot;;
            //string infn = path + @&quot;CELLSNET-24389\ScatterConnectedXls.xlsx&quot;;
            //string outfn = path + @&quot;CELLSNET-24389\ScatterConnected_out.xlsx&quot;;

            Workbook workbook = new Workbook();

            Style style = workbook.DefaultStyle;
            style.Font.Name = &quot;Tahoma&quot;;
            workbook.DefaultStyle = style;

            CreateStaticData(workbook);
            CreateCellsFormatting(workbook);
            CreateStaticReport(workbook);
            workbook.Save(outfnXlsx, SaveFormat.Xlsx);
            workbook.Save(outfnXls, SaveFormat.Excel97To2003);

            //Workbook workbook = new Workbook(infn);
            //workbook.Save(outfn, SaveFormat.Xlsx);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


