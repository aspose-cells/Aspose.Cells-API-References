---
title: Validation.Operator
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the operator for the data validation
type: docs
url: /net/aspose.cells/validation/operator/
---
## Validation.Operator property

Represents the operator for the data validation.

```csharp
public OperatorType Operator { get; set; }
```

### Examples

```csharp
// Called: val.Operator = OperatorType.Between;
public void Validation_Property_Operator()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 4; i++)
    {
        cells[i, 0].PutValue("VldtItem" + i);
    }
    Aspose.Cells.Range rng = cells.CreateRange("A1:A4");
    rng.Name = "MyRange508";
    Util.SetHintMessage(cells["B1"], "Please check the validation in Sheet2!A1, there should be a list to be chosen");

    Worksheet ws = wb.Worksheets.Add("Sheet2");
    CellArea ca = CellArea.CreateCellArea("A1", "A5");

    int idx = ws.Validations.Add(ca);
    Validation val = ws.Validations[idx];

    val.ErrorMessage = "This is error.";
    val.Formula1 = "=MyRange508";
    val.Operator = OperatorType.Between;
    val.Type = ValidationType.List;
    Util.SaveManCheck(wb, "", "example.xls");
}
```

### See Also

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


