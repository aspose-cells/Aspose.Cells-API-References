---
title: SeriesCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Clears the collection
type: docs
url: /net/aspose.cells.charts/seriescollection/clear/
---
## SeriesCollection.Clear method

Clears the collection

```csharp
public void Clear()
```

### Examples

```csharp
// Called: ch.NSeries.Clear();
[Test]
         //http://www.aspose.com/community/forums/thread/344750/copying-charts.aspx
         public void Method_Clear()
         {
             Console.WriteLine("testCELLSNET_40128()");
             string infn = path + @"CELLSNET-40128\Book1_40128.xlsx";
             string outfn = destpath + @"Book1_40128.out.png";
             string outfn1 = destpath + @"Book1_40128.out.xlsx";

             Workbook wb1 = new Workbook(infn);
             Workbook wb2 = new Workbook();
             Worksheet sh = wb1.Worksheets["Sheet1"];
             wb2.Worksheets.Add();
             wb2.Worksheets[0].Copy(sh);

             sh = wb1.Worksheets["Chart1"];
             wb2.Worksheets.Add();
             Int32 i = 1;
             wb2.Worksheets[i].Copy(sh);
             Aspose.Cells.Charts.Chart ch = wb2.Worksheets[i].Charts[0];
             ch.NSeries.Clear();
             ch.NSeries.Add("Sheet1!B2:C3", false);
             ch.NSeries.CategoryData = "Sheet1!B1:C1";
             ch.Style = sh.Charts[0].Style;
             for (int j = 0; j < ch.NSeries.Count; j++)
             {
                 ch.NSeries[j].Name = "=Sheet1!" + CellsHelper.CellIndexToName(1 + j, 0);
             }
             wb2.Save(outfn1);
             wb2.Worksheets[1].Charts[0].ToImage(outfn);
#if WTEST
             Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
         }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


