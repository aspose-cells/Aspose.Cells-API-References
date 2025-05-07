---
title: Validation.ErrorMessage
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the data validation error message
type: docs
url: /net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

Represents the data validation error message.

```csharp
public string ErrorMessage { get; set; }
```

### Examples

```csharp
// Called: val.ErrorMessage = "This is error.";
[Test]
        public void Property_ErrorMessage()
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
            Util.SaveManCheck(wb, "", "N46193_res.xls");
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


