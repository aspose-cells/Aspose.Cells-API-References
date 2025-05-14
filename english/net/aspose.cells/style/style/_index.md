---
title: Style.Style
second_title: Aspose.Cells for .NET API Reference
description: Style constructor. Initializes a new instance of the Style class
type: docs
url: /net/aspose.cells/style/style/
---
## Style constructor

Initializes a new instance of the [`Style`](../) class.

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Remarks

NOTE: This constructor is now obsolete. Instead, please use CellsFactory.CreateStyle() method. This property will be removed 6 months later since October 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: var style = new Style(); // this used to work in 20.04 but causes corruption starting with 20.06
private static void Style_Constructor(Workbook workbook, List<string> columns)
        {
            var pivotSheet = workbook.Worksheets.Add("Pivot1");
            var pivotTableIndex = pivotSheet.PivotTables.Add(string.Format("'{0}'!{1}", "Pivot1", "Data0"), "A5", "Pivot");
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            foreach (var column in columns)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Row, column);
            }
            pivotTable.CalculateData();

            foreach (var column in columns)
            {
                var cell = pivotTable.GetCellByDisplayName(column);
                if (cell == null)
                    continue;
                var style = new Style(); // this used to work in 20.04 but causes corruption starting with 20.06
                                         // style.BackgroundColor = Color.Red;
                pivotTable.Format(cell.Row, cell.Column, style);
            }
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


