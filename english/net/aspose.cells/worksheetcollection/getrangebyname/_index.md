---
title: WorksheetCollection.GetRangeByName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets Range object by predefined name
type: docs
url: /net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Gets Range object by pre-defined name.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range. |

### Return Value

Range object.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range range = wb.Worksheets.GetRangeByName(rangeName);
private Aspose.Cells.Range WorksheetCollection_Method_GetRangeByName(Workbook wb, string rangeName, bool throwIfNotFound)
        {
            Aspose.Cells.Range range = wb.Worksheets.GetRangeByName(rangeName);
            if (range == null && throwIfNotFound)
            {
                throw new ApplicationException(string.Format("No range exists with name '{0}'", rangeName));
            }

            return range;
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Gets [`Range`](../../range/) by pre-defined name or table's name

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range or table's name. |
| currentSheetIndex | Int32 | The sheet index. -1 represents global . |
| includeTable | Boolean | Indicates whether checking all tables. |

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


