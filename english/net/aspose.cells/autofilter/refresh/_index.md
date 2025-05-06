---
title: AutoFilter.Refresh
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Refresh auto filters to hide or unhide the rows
type: docs
url: /net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

Refresh auto filters to hide or unhide the rows.

```csharp
public int[] Refresh()
```

### Return Value

Returns all hidden rows' indexes.

### Examples

```csharp
// Called: filter.Refresh();
[Test]
        public void Method_Refresh()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET55309.xlsx&quot;);
            var worksheet = wb.Worksheets[0];
         

            var filter = worksheet.AutoFilter;
            filter.MatchBlanks(1);
            Assert.IsFalse(worksheet.Cells.Rows[6].IsHidden);

            filter.Refresh();
            Assert.IsFalse(worksheet.Cells.Rows[6].IsHidden);

            filter.AddFilter(1, &quot;超短期融资债券&quot;);
            filter.Refresh();
            Assert.IsFalse(worksheet.Cells.Rows[6].IsHidden);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

Gets all hidden rows' indexes.

```csharp
public int[] Refresh(bool hideRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| hideRows | Boolean | If true, hide the filtered rows. |

### Return Value

Returns all hidden rows indexes.

### Examples

```csharp
// Called: wbDesigner.Workbook.Worksheets[0].AutoFilter.Refresh(true);
[Test]
        public void Method_Boolean_()
        {
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.None;
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;
            WorkbookDesigner wbDesigner = new WorkbookDesigner(
                new Workbook(Constants.sourcePath + &quot;AutoFilter/CellsNet46369.xlsx&quot;, loadOptions));

            //Add values to the rows in the excel which are filtered in the tempalte file
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;A13&quot;].Value = 1000009;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;C13&quot;].Value = DateTime.Now.ToShortDateString();
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;D13&quot;].Value = &quot;DDDDDDDDDDDDDDD&quot;;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;E13&quot;].Value = &quot;EEEEEEEEEEEEEEEEEEE&quot;;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;F13&quot;].Value = 12;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;G13&quot;].Value = 15;

            wbDesigner.Workbook.Worksheets[0].Cells[&quot;A14&quot;].Value = 1000010;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;C14&quot;].Value = DateTime.Now.ToShortDateString();
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;D14&quot;].Value = &quot;DDDDDDDDDDDDDDD1&quot;;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;E14&quot;].Value = &quot;EEEEEEEEEEEEEEEEEEE1&quot;;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;F14&quot;].Value = 14;
            wbDesigner.Workbook.Worksheets[0].Cells[&quot;G14&quot;].Value = 16;
            //Recalculate the sheet
            wbDesigner.Workbook.CalculateFormula();
            //set the filter values
            wbDesigner.Workbook.Worksheets[0].AutoFilter.Filter(0, &quot;FALSE&quot;);
            // Refresh the filter to hide or show the rows
            wbDesigner.Workbook.Worksheets[0].AutoFilter.Refresh(true);
            Console.WriteLine(wbDesigner.Workbook.Worksheets[0].Cells.GetRowHeightPixel(13));
            //The issue. Saved version doesnt maintain the row height.
            //Only the visible row in the tempalte file is maintaining the row height.
            //The rows to which values are added are not maintaining the row height
            //Intempalte file the row height is set to 25
            Util.ReSave(wbDesigner.Workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + &quot;CellsNet46369.xlsx&quot;);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


