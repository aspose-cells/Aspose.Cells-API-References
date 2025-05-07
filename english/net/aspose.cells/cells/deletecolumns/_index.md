---
title: Cells.DeleteColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes several columns
type: docs
url: /net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Deletes several columns.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: cells.DeleteColumns(0, 0, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    cells[i, j].PutValue(i * 3 + j);
                }
            }
            cells.DeleteColumns(0, 0, true);
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    AssertHelper.AreEqual(i * 3 + j, cells[i, j].IntValue, CellsHelper.CellIndexToName(i, j));
                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Deletes several columns.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| options | DeleteOptions | Options for the deleting operation |

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


