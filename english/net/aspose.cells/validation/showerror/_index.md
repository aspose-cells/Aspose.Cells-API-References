---
title: Validation.ShowError
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether the data validation error message will be displayed whenever the user enters invalid data
type: docs
url: /net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indicates whether the data validation error message will be displayed whenever the user enters invalid data.

```csharp
public bool ShowError { get; set; }
```

### Examples

```csharp
// Called: validation.ShowError = true;
[Test, Category(&quot;Bug&quot;)]
        public void Property_ShowError()
        {
            String namedRange = &quot;arange34&quot;;
            Workbook workbook = new Workbook();
            Worksheet pickListSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            pickListSheet.Cells[0, 0].PutValue(&quot;value 1&quot;);
            pickListSheet.Cells[1, 0].PutValue(&quot;value 2&quot;);
            pickListSheet.Cells[2, 0].PutValue(&quot;value 3&quot;);
            Aspose.Cells.Range range = pickListSheet.Cells.CreateRange(0, 0, 3, 1);
            range.Name = namedRange;
            CellArea area = new CellArea();
            area.StartRow = 3;
            area.StartColumn = 3;
            area.EndRow = 3;
            area.EndColumn = 3;

            Worksheet worksheet = workbook.Worksheets[0];
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Operator = OperatorType.None;
            validation.InCellDropDown = true;
            validation.Formula1 = &quot;=&quot; + namedRange;
            validation.ShowError = true;
            validation.AlertStyle = ValidationAlertType.Warning;
            validation.ErrorTitle = &quot;Warning&quot;;
            validation.ErrorMessage = &quot;Please select a value from the list&quot;;
           
            worksheet.Cells[3, 3].PutValue(&quot;value 2&quot;);
            workbook.Save(Constants.destPath + &quot;wrk1.xml&quot;, SaveFormat.SpreadsheetML);
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


