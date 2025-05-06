---
title: FormatConditionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets the formatting condition by index
type: docs
url: /net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Gets the formatting condition by index.

```csharp
public FormatCondition this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | the index of the formatting condition to return. |

### Return Value

the formatting condition

### Examples

```csharp
// Called: FormatCondition fc = fcs[conditionIndex];
[Test]
        public void Property_Int32_()
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
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, &quot;-50&quot;, &quot;-1&quot;);  
            FormatCondition fc = fcs[conditionIndex];              
            fc.Style.Font.Color = Color.Red;                
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, &quot;0&quot;, &quot;50&quot;);  
            fc = fcs[conditionIndex];                 
            fc.Style.Font.Color = Color.Green;        
            //Saving the Excel file        
            workbook.Save(Constants.destPath + &quot;Test_160826.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_160826.xls&quot;); 
          
        }
```

### See Also

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


