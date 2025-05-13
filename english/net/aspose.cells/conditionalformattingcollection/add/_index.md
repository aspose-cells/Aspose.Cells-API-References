---
title: ConditionalFormattingCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingCollection method. Adds a FormatConditions to the collection
type: docs
url: /net/aspose.cells/conditionalformattingcollection/add/
---
## ConditionalFormattingCollection.Add method

Adds a FormatConditions to the collection.

```csharp
public int Add()
```

### Return Value

FormatConditions object index.

### Examples

```csharp
// Called: int index = sheet.ConditionalFormattings.Add();
public void ConditionalFormattingCollection_Method_Add()
{
    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    int index = sheet.ConditionalFormattings.Add();
    FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
    //Sets the conditional format range.
    CellArea ca = new CellArea();
    ca.StartRow = 0;
    ca.EndRow = 0;
    ca.StartColumn = 0;
    ca.EndColumn = 0;
    fcs.AddArea(ca);
    //Adds condition.
    int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.NotBetween, "10", "100");
    FormatCondition fc = fcs[conditionIndex];
    fc.Style.BackgroundColor = Color.Red;

    checkOperatorType_NotBetween(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkOperatorType_NotBetween(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkOperatorType_NotBetween(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    checkOperatorType_NotBetween(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


