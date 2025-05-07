---
title: Cell.GetValidationValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the value of validation which applied to this cell
type: docs
url: /net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Gets the value of validation which applied to this cell.

```csharp
public bool GetValidationValue()
```

### Examples

```csharp
// Called: bool isValid = age.GetValidationValue(); // isValid is true
[Test]
        public void Method_GetValidationValue()
        {
            var book = new Workbook(Constants.sourcePath + "CellsNet45532_2.xlsx");
            book.CalculateFormula();

            Worksheet sheetBla = book.Worksheets["Sheet2"];

            Cell age = sheetBla.Cells["B1"];
            //age.PutValue("-60", true, false);//Not Ok 
            //age.PutValue(-60);//Not Ok 
            //age.PutValue(15);//Not Ok 
            age.PutValue(101);//Not Ok 

            book.CalculateFormula();

            bool isValid = age.GetValidationValue(); // isValid is true 
            Assert.IsFalse(isValid);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


