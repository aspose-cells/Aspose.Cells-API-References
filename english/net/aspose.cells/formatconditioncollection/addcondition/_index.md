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
// Called: int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
public void FormatConditionCollection_Method_AddCondition()
{
    Workbook workbook = new Workbook(); 
    Worksheet sheet = workbook.Worksheets[0];              
    //Adds an empty conditional formatting             
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
    int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");  
    FormatCondition fc = fcs[conditionIndex];              
    fc.Style.Font.Color = Color.Red;                
    conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");  
    fc = fcs[conditionIndex];                 
    fc.Style.Font.Color = Color.Green;        
    //Saving the Excel file        
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls"); 
          
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
// Called: idx = conds.AddCondition(FormatConditionType.ColorScale);
public void FormatConditionCollection_Method_AddCondition()
{
    Console.WriteLine("FormatConditionCollection_Method_AddCondition()");
    string outfn = Constants.destPath + "Test_NewCndFmtDefaultColor_out.xlsx";

    Workbook book = new Workbook();
    Worksheet sheet1 = book.Worksheets[0];

    FormatConditionCollection conds = GetFormatCondition(sheet1, "A1:C2", Color.Yellow);
    int idx = conds.AddCondition(FormatConditionType.IconSet);

    conds = GetFormatCondition(sheet1, "A5:C6", Color.Pink);
    idx = conds.AddCondition(FormatConditionType.ColorScale);
    //FormatCondition cond = conds[idx];

    book.Save(outfn);
}
```

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


