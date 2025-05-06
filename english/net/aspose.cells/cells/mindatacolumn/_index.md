---
title: Cells.MinDataColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum column index of cell which contains data
type: docs
url: /net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Minimum column index of cell which contains data.

```csharp
public int MinDataColumn { get; }
```

### Remarks

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### Examples

```csharp
// Called: int index = sheet.ListObjects.Add(sheet.Cells.MinDataRow, sheet.Cells.MinDataColumn,
[Test]
        public void Property_MinDataColumn()
        {
            string validator = &quot;=[@Column A] &gt; 10&quot;;

            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            sheet.Cells[&quot;A1&quot;].Value = &quot;Column A&quot;;
            sheet.Cells[&quot;B1&quot;].Value = &quot;Column B&quot;;

            sheet.Cells[&quot;A2&quot;].Value = 10;
            sheet.Cells[&quot;A3&quot;].Value = 20;
            sheet.Cells[&quot;A4&quot;].Value = 30;

            int index = sheet.ListObjects.Add(sheet.Cells.MinDataRow, sheet.Cells.MinDataColumn,
                sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true);
            var table = sheet.ListObjects[index];
            var column = table.ListColumns[table.ListColumns.Count - 1];

            sheet.Cells[&quot;B2&quot;].Formula = validator;
            sheet.Cells[&quot;B3&quot;].Formula = validator;
            sheet.Cells[&quot;B4&quot;].Formula = validator;

            ValidationCollection validations = sheet.Validations;
            Aspose.Cells.Range r = column.Range;
            CellArea area = CellArea.CreateCellArea(r.FirstRow + 1, r.FirstColumn,
                r.FirstRow + r.RowCount - 1, r.FirstColumn);
            Validation validation = validations[validations.Add(area)];
            validation.Type = ValidationType.Custom;
            validation.ShowError = false;
            validation.Formula1 = validator;

            wb.CalculateFormula();

            Assert.IsFalse(sheet.Cells[&quot;B2&quot;].BoolValue, &quot;B2.Value&quot;);
            Assert.IsTrue(sheet.Cells[&quot;B3&quot;].BoolValue, &quot;B3.Value&quot;);
            Assert.IsTrue(sheet.Cells[&quot;B4&quot;].BoolValue, &quot;B4.Value&quot;);

            Assert.IsFalse(sheet.Cells[&quot;B2&quot;].GetValidationValue(), &quot;B2.Validation&quot;);
            Assert.IsTrue(sheet.Cells[&quot;B3&quot;].GetValidationValue(), &quot;B3.Validation&quot;);
            Assert.IsTrue(sheet.Cells[&quot;B4&quot;].GetValidationValue(), &quot;B4.Validation&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


