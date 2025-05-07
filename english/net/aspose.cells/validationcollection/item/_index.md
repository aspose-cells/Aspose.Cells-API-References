---
title: ValidationCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection property. Gets the Validation element at the specified index
type: docs
url: /net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Gets the [`Validation`](../../validation/) element at the specified index.

```csharp
public Validation this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Validation validation = sheet.Validations[index];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[1, 1].Formula = "=Now()";
            CellArea cellarea = common.setCellArea(0, 0, 1, 1);
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            validation.Type = ValidationType.Time;
            validation.Operator = OperatorType.Equal;
            validation.Formula1 = "=A1";
         
            workbook.CalculateFormula();

            checkValidationType_Time(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkValidationType_Time(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkValidationType_Time(workbook);
           workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkValidationType_Time(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


