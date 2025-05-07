---
title: CellValue.Type
second_title: Aspose.Cells for .NET API Reference
description: CellValue property. Gets/sets the type of cell value
type: docs
url: /net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

Gets/sets the type of cell value.

```csharp
public CellValueType Type { get; set; }
```

### Examples

```csharp
// Called: cellValue.Type = CellValueType.IsNumeric;
public static void Property_Type()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a CellValue instance
            CellValue cellValue = new CellValue();

            // Set the type and value of the cell
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Assign the CellValue to a cell in the worksheet
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Save the workbook
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


