---
title: Row.IsBlank
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row contains any data
type: docs
url: /net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Indicates whether the row contains any data

```csharp
public bool IsBlank { get; }
```

### Examples

```csharp
// Called: if (currRow.IsBlank)
private bool Property_IsBlank(Worksheet sheet)
        {
            //You can customize the number of rows between outliers and master data regions
            int abnormalCount = 200000;

            int total = 0;
            bool isExistAbnormalCell = false;
            RowCollection rows = sheet.Cells.Rows;
            IEnumerator rowIEnum = rows.GetEnumerator();

            while (rowIEnum.MoveNext())
            {
                Row currRow = (Row)rowIEnum.Current;
                if (currRow.IsBlank)
                {
                    total++;
                }
                else
                {
                    total = 0;
                }

                if (total &gt; abnormalCount)
                {
                    isExistAbnormalCell = true;
                    break;
                }
            }

            return isExistAbnormalCell;
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


