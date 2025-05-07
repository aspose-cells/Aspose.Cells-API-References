---
title: FormatConditionCollection.RangeCount
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets count of conditionally formatted ranges
type: docs
url: /net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Gets count of conditionally formatted ranges.

```csharp
public int RangeCount { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, worksheet.ConditionalFormattings[0].RangeCount);
[Test]
        public void Property_RangeCount()
        {
            var wb = new Workbook(Constants.sourcePath + "Net53737.xlsx");
            Worksheet worksheet = wb.Worksheets[0];
            var ca = new CellArea();
            ca.StartRow = 10;
            ca.EndRow = 202;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // insert rows example
           // worksheet.Cells.InsertRows(10, 193, false);
            for (var r = 0; r < 194; r++)
            {
                if (r > 0)
                {
                    // copy styling and formulas
                    worksheet.Cells.CopyRow(worksheet.Cells, 9, 9 + r);
                }
            }
            Assert.AreEqual(1, worksheet.ConditionalFormattings.Count);
            Assert.AreEqual(1, worksheet.ConditionalFormattings[0].RangeCount);
            wb.Settings.FormulaSettings.CalculateOnOpen = true;
            wb = Util.ReSave(wb, SaveFormat.Xlsx);//wb.Save(Constants.destPath + "Net53737_2.xlsx");
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


