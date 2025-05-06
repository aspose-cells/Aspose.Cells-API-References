---
title: FormatConditionCollection.AddCondition
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a formatting condition
type: docs
url: /net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Adds a formatting condition.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | The type of format condition. |
| operatorType | OperatorType | The operator type |
| formula1 | String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | String | The value or expression associated with conditional formatting. The input format is same with formula1 |

### Return Value

Formatting condition object index;

### Examples

```csharp
// Called: int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, &amp;quot;0&amp;quot;, &amp;quot;100&amp;quot;);
[Test]
        public void Method_String_()
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
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, &quot;0&quot;, &quot;100&quot;);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            checkOperatorType_Between(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkOperatorType_Between(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkOperatorType_Between(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkOperatorType_Between(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Add a format condition.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | FormatConditionType | Format condition type. |

### Return Value

Formatting condition object index;

### Examples

```csharp
// Called: fcc.AddCondition(FormatConditionType.UniqueValues);
[Test]
        public void Method_FormatConditionType_()
        {
            TestJ42914Sub(true);
            TestJ42914Sub(false);
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1048575, 0));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            fcc[0].Style.Font.Size = 16;
            fcc.AddCondition(FormatConditionType.UniqueValues);
            fcc[1].Style.Font.Size = 22;
            Console.WriteLine(&quot;LargeDataSetUniDupFormatCondtion: initializing large cells dataset...&quot;);
            for (int i = 2; i &lt; 30000; i++)
            {
                if (i%1000 == 0)
                {
                    continue;
                }
                cells[i, 0].PutValue(&quot;stringvalueduplicateanduniquetest&quot; + i);
            }
            cells[30001, 0].PutValue(&quot;stringvalueduplicateanduniquetest2&quot;);
            sheet.PageSetup.PrintArea = &quot;$A$1:$A$5&quot;;
            Console.WriteLine(&quot;finished. Test performance of saving...&quot;);
            TimePerformance monitor = new TimePerformance(140);
            monitor.StartPerfTest();
            wb.Save(new MemoryStream(), SaveFormat.Pdf);
            monitor.FinishPerfTest(&quot;LargeDataSetUniDupFormatCondtion&quot;);
        }
```

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


