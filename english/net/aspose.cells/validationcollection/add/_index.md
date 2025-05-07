---
title: ValidationCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection method. Adds a data validation to the collection
type: docs
url: /net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Adds a data validation to the collection.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Return Value

[`Validation`](../../validation/) object index.

### Remarks

NOTE: This member is now obsolete. Instead, please use ValidationCollection.Add(CellArea) method. This property will be removed 12 months later since JANUARY 2015. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Adds a data validation to the collection.

```csharp
public int Add(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The area contains this validation. |

### Return Value

[`Validation`](../../validation/) object index.

### Examples

```csharp
// Called: int index = sheet.Validations.Add(cellarea);
[Test]
        public void Method_CellArea_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            CellArea cellarea = common.setCellArea(0, 0, 1, 1);
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";

          

            checkValidationType_List(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkValidationType_List(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkValidationType_List(workbook);
           workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkValidationType_List(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


