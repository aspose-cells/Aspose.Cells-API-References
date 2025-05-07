---
title: StyleFlag.Locked
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Locked setting will be applied
type: docs
url: /net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Locked setting will be applied.

```csharp
public bool Locked { get; set; }
```

### Examples

```csharp
// Called: styleFlag.Locked = true;
private static void Property_Locked(Aspose.Cells.Range range, DataTable tbl)
        {
            Worksheet workSheet = range.Worksheet;
            Cells cells = workSheet.Cells;
            Workbook workbook = workSheet.Workbook;

            Cell cell2 = cells[0, 0];
            DataColumn cssColumn = tbl.Columns["Css"];
            DataColumn cssTargetColumn = tbl.Columns["Additional"];

            bool useHeader = true;
            int useHeaderOffset = useHeader ? 1 : 0;
            int rowIndex = 0;
            int colIndex = cssTargetColumn.Ordinal;
            foreach (DataRow row in tbl.Rows)
            {
                string cssClass = row[cssColumn] as string;
                if (!string.IsNullOrEmpty(cssClass))
                {
                    Cell cell = cells[rowIndex + range.FirstRow + useHeaderOffset, range.FirstColumn + colIndex];
                    Style style = workbook.GetNamedStyle(cssClass);
                    if (style == null)
                    {
                        throw new InvalidOperationException(string.Format("No such style exists: '{0}'.", cssClass));
                    }

                    StyleFlag styleFlag = new StyleFlag();
                    styleFlag.Borders = true;
                    styleFlag.CellShading = true;
                    styleFlag.Font = true;
                    styleFlag.Locked = true;
                    cell.SetStyle(style, true);
                    cell.GetStyle().Name = "IW_Kalle";

                    Cell cellCopy = cells[rowIndex + 1, range.FirstColumn + colIndex + 5];
                    cellCopy.SetStyle(cell.GetStyle(), true);

                    rowIndex++;
                }
            }
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


