---
title: AutoFitterOptions.AutoFitWrappedTextType
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the type of auto fitting wrapped text
type: docs
url: /net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Gets and sets the type of auto fitting wrapped text.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Examples

```csharp
// Called: options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;
[Test]
        public void Property_AutoFitWrappedTextType()
        {
            Workbook workbook = new Workbook();
            //Get the first (default) worksheet.
            Worksheet sheet = workbook.Worksheets[0];
            //Get the cells in the sheet.
            Cells cells = sheet.Cells;
            //Merging two cells (A5:E5)into a single cell(B5).
            cells.Merge(4, 0, 1, 5);

            Cell cell = sheet.Cells[4, 0];
            Style style = sheet.Cells[4, 0].GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            //Put some value into the merged cell.
            cells["A5"].PutValue("Please select the conversion rate and velocity between each stage for the waterfall type you selected in the prior question. For reference, we have included definitions of each stage.Marketing through tele – Marketing sources an inquiry that passes through a telequalification function before acceptance/rejection by a field sales force.  Inquiry: The total number of raw responses or hand-raisers to an outbound or inbound marketing activity. Relatively little is known about the prospect at this point. Automation qualified lead (AQL): A lead that has been qualified via an automated system or tool and is deemed ready for a receiving function to work. Teleprospecting accepted lead (TAL): A lead that has been formally accepted by the teleprospecting function, which is then compelled to work the lead in a given timeframe to promote or disqualify it. Teleprospecting qualified lead (TQL): A lead that has been qualified via teleprospecting and is deemed ready for a receiving function (e.g. field rep, channel partner) to work. Sales accepted lead (SAL): A lead that has been formally accepted by the sales function, which is then compelled to work the lead in a given timeframe to promote or disqualify it. Sales qualified lead (SQL): A lead that has evolved into opportunities – complete with estimated revenue and timeframe to close. Won business: An opportunity that has converted to a closed/won deal.");

            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            sheet.AutoFitRows(options);
            workbook.Save(Constants.destPath + "CellsNet50157_1.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet50157_1.xlsx");
            Assert.IsFalse(workbook.Worksheets[0].Cells.Rows[4].IsHeightMatched);
            Assert.AreEqual(459,workbook.Worksheets[0].Cells.GetRowHeightPixel(4));
        }
```

### See Also

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


