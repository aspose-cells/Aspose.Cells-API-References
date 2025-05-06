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
// Called: var validationB = newWsB.Validations[newWsB.Validations.Add(cellAreaB)];
public static void Method_CellArea_()
        {
            var wb = new Workbook();

            var newWsA = wb.Worksheets[0];
            newWsA.Name = &quot;SheetA&quot;;
            newWsA.Cells[0, 0].Value = &quot;A&quot;;
            newWsA.Cells[1, 0].Value = &quot;B&quot;;
            newWsA.Cells[2, 0].Value = &quot;C&quot;;
            newWsA.Cells[3, 0].Value = &quot;D&quot;;
            newWsA.Cells[4, 0].Value = &quot;E&quot;;

            var newWsB = wb.Worksheets.Add(&quot;SheetB&quot;);
            newWsB.Cells[0, 0].Value = &quot;AA&quot;;
            newWsB.Cells[1, 0].Value = &quot;BB&quot;;
            newWsB.Cells[2, 0].Value = &quot;CC&quot;;
            newWsB.Cells[3, 0].Value = &quot;DD&quot;;
            newWsB.Cells[4, 0].Value = &quot;EE&quot;;

            var cellAreaA = new CellArea();
            cellAreaA.StartRow = 0;
            cellAreaA.StartColumn = 1;
            cellAreaA.EndRow = 1;
            cellAreaA.EndColumn = 1;
            var validationA = newWsA.Validations[newWsA.Validations.Add(cellAreaA)];
            validationA.Type = ValidationType.List;
            validationA.Formula1 = @&quot;=SheetB!$A:$A&quot;;

            var cellAreaB = new CellArea();
            cellAreaB.StartRow = 0;
            cellAreaB.StartColumn = 1;
            cellAreaB.EndRow = 1;
            cellAreaB.EndColumn = 1;
            var validationB = newWsB.Validations[newWsB.Validations.Add(cellAreaB)];
            validationB.Type = ValidationType.List;
            validationB.Formula1 = @&quot;=SheetA!$A:$A&quot;;

            OutputValidations(wb, &quot;CreateBook&quot;);
            Util.ReSave(wb, SaveFormat.Xlsx);
            //wb.Save(Constants.destPath + &quot;CellsNet45795.xlsx&quot;);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


