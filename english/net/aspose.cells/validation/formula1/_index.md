---
title: Validation.Formula1
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the value or expression associated with the data validation
type: docs
url: /net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Represents the value or expression associated with the data validation.

```csharp
public string Formula1 { get; set; }
```

### Examples

```csharp
// Called: validation.Formula1 = "2009-1-1";
[Test]
        public void Property_Formula1()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            CellArea cellarea = common.setCellArea(0, 0, 1, 1);
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            validation.Type = ValidationType.Date;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "2009-1-1";
            validation.Formula2 = "2009-12-31";
           

            checkValidationType_Date(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkValidationType_Date(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkValidationType_Date(workbook);
           workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkValidationType_Date(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


