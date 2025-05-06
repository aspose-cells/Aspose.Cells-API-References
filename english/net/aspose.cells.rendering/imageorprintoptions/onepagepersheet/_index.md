---
title: ImageOrPrintOptions.OnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. If OnePagePerSheet is true  all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: imgOption.OnePagePerSheet = true;
[Test]
        public void Property_OnePagePerSheet()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA41170_&quot;;
            Workbook workbook = new Workbook(filePath + &quot;test.xltx&quot;);
            WorksheetCollection worksheets = workbook.Worksheets;
            Cells cells = worksheets[&quot;Data&quot;].Cells;

            FillRow(cells, 1, &quot;Full Decommission&quot;, 1, null, 1, null, 1, 1);
            FillRow(cells, 2, &quot;Design 1 (Phase 1- 3)&quot;, null, 1, 1, 1, null, null);
            FillRow(cells, 3, &quot;Design 1 (Phase 1- 3) Fallout Candidate&quot;, null, null, 1, 1, 1, 1);
            FillRow(cells, 4, &quot;MW Backhaul or POP&quot;, 1, null, null, 1, null, 1);
            FillRow(cells, 5, &quot;RF Repeater&quot;, 1, 1, null, null, 1, 1);
            FillRow(cells, 6, &quot;License Protection&quot;, null, 1, null, 1, null, 1);
            FillRow(cells, 7, &quot;Full Decommission&quot;, 1, null, 1, null, 1, 1);
            FillRow(cells, 8, &quot;Design 1 (Phase 1- 3)&quot;, null, 1, 1, 1, null, null);
            FillRow(cells, 9, &quot;Design 1 (Phase 1- 3) Fallout Candidate&quot;, null, null, 1, 1, 1, 1);
            FillRow(cells, 10, &quot;MW Backhaul or POP&quot;, 1, null, null, 1, null, 1);
            FillRow(cells, 11, &quot;RF Repeater&quot;, 1, 1, null, null, 1, 1);
            FillRow(cells, 12, &quot;License Protection&quot;, null, 1, null, 1, null, 1);
            FillRow(cells, 13, &quot;Full Decommission&quot;, 1, null, 1, null, 1, 1);
            FillRow(cells, 14, &quot;Design 1 (Phase 1- 3)&quot;, null, 1, 1, 1, null, null);
            FillRow(cells, 15, &quot;Design 1 (Phase 1- 3) Fallout Candidate&quot;, null, null, 1, 1, 1, 1);
            FillRow(cells, 16, &quot;MW Backhaul or POP&quot;, 1, null, null, 1, null, 1);
            FillRow(cells, 17, &quot;RF Repeater&quot;, 1, 1, null, null, 1, 1);
            FillRow(cells, 18, &quot;License Protection&quot;, null, 1, null, 1, null, 1);

            for (int i = 0; i &lt; worksheets.Count; i++)
            {
                Worksheet worksheet = worksheets[i];

                PivotTableCollection pivotTables = worksheet.PivotTables;
                for (int j = 0; j &lt; pivotTables.Count; j++)
                {
                    PivotTable pivotTable = pivotTables[j];
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                }
            }

            for (int i = 0; i &lt; worksheets.Count; i++)
            {
                Worksheet worksheet = worksheets[i];

                ChartCollection charts = worksheet.Charts;
                for (int j = 0; j &lt; charts.Count; j++)
                {
                    Chart chart = charts[j];
                    chart.RefreshPivotData();
                    chart.Calculate();
                }
            }

            ImageOrPrintOptions imgOption = new ImageOrPrintOptions();
#if !NETCOREAPP2_0
            imgOption.ImageType = ImageType.Jpeg;
#endif
            imgOption.HorizontalResolution = 300;
            imgOption.VerticalResolution = 300;
            imgOption.OnePagePerSheet = true;

            SheetRender sr = null;
            sr = new SheetRender(worksheets[&quot;Image1&quot;], imgOption);
            sr.ToImage(0, Constants.PivotTableDestPath + @&quot;JAVA41170.jpeg&quot;);

            workbook.Save(Constants.PivotTableDestPath + @&quot;JAVA41170.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


