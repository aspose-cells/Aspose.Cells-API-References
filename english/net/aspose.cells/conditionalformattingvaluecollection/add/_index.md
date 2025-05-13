---
title: ConditionalFormattingValueCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValueCollection method. Adds ConditionalFormattingValue object
type: docs
url: /net/aspose.cells/conditionalformattingvaluecollection/add/
---
## ConditionalFormattingValueCollection.Add method

Adds [`ConditionalFormattingValue`](../../conditionalformattingvalue/) object.

```csharp
public int Add(FormatConditionValueType type, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionValueType | The value type. |
| value | String | The value. |

### Return Value

Returns the index of new object in the list.

### Examples

```csharp
// Called: int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");
public static void ConditionalFormattingValueCollection_Method_Add()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Sets the conditional format range
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Adds condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];

            // Get Icon Set
            IconSet iconSet = cond.IconSet;

            // Set Icon Type
            iconSet.Type = IconSetType.Arrows3;

            // Get the CFValueObjects instance
            ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

            // Add a new ConditionalFormattingValue to the collection
            int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");

            // Access the newly added ConditionalFormattingValue
            ConditionalFormattingValue cfv = cfvos[cfvIndex];

            // Modify properties of the ConditionalFormattingValue
            cfv.Value = 75;
            cfv.Type = FormatConditionValueType.Percent;
            cfv.IsGTE = true;

            // Put Cell Values
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Saving the Excel file
            workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
            workbook.Save("ConditionalFormattingValueCollectionExample.pdf");
        }
```

### See Also

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


