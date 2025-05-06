---
title: TickLabels.NumberFormatLinked
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. True if the number format is linked to the cells so that the number format changes in the labels when it changes in the cells
type: docs
url: /net/aspose.cells.charts/ticklabels/numberformatlinked/
---
## TickLabels.NumberFormatLinked property

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(c.ValueAxis.TickLabels.NumberFormatLinked);
[Test]
        //Mo Sujun bug
        public void Property_NumberFormatLinked()
        {
            Console.WriteLine(&quot;Property_NumberFormatLinked()&quot;);
            string infn = path + @&quot;LinkSource\Personal+Financial+Planning+Modelling+-+Websheets.xlsm&quot;;
            string outfn = Constants.destPath + @&quot;Personal+Financial+Planning+Modelling+-+Websheets_out.xlsm&quot;;

            Workbook workbook = new Workbook(infn);

            ChartCollection charts = workbook.Worksheets[&quot;Results - Docs - Comments on FS&quot;].Charts;
            Chart c = charts[&quot;Chart 1026&quot;];
            Console.WriteLine(c.ValueAxis.TickLabels.NumberFormatLinked);

            workbook.Save(outfn, SaveFormat.Xlsm);
        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


