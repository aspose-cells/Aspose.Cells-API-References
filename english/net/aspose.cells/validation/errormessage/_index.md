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
// Called: v.ErrorMessage = &amp;quot;The number is not valid.&amp;quot;;
[Test]
       public void Property_ErrorMessage()
       {
           Workbook wb = new Workbook();
           Worksheet ws = wb.Worksheets[0];
           Cells wsCells = ws.Cells;
       

           int row = 0, col = 0;

           for (row = 0; row &lt; 10; row++)
           {
               for (col = 0; col &lt; 10; col++)
               {
                   wsCells[row, col].PutValue(Convert.ToDecimal(row + col));
               }
           }
           CellArea cellArea = new CellArea();
           cellArea.EndColumn = col;
           cellArea.EndRow = row;
           cellArea.StartColumn = 0;
           cellArea.StartRow = 0;
           int valId = ws.Validations.Add(cellArea);
           Validation v = ws.Validations[valId];

           v.Type = ValidationType.Decimal;
           v.Operator = OperatorType.Between;
           v.Formula1 = &quot;0&quot;;
           v.Formula2 = &quot;9999999&quot;;
           v.ErrorMessage = &quot;The number is not valid.&quot;;
           v.ErrorTitle = &quot;Error Title&quot;;
           v.AlertStyle = ValidationAlertType.Stop;
           v.ShowError = true;

          
           Assert.AreEqual(ws.Validations.Count, 1);

       }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


