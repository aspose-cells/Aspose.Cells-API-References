---
title: Workbook.Combine
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Combines another Workbook object
type: docs
url: /net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Combines another Workbook object.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | Workbook | Another Workbook object. |

### Remarks

Merge Excel, ODS , CSV and other files to one file.

### Examples

```csharp
// Called: SourceBook1.Combine(SourceBook2);
[Test]
        public void Method_Workbook_()
        {
            Workbook SourceBook1 = new Workbook(Constants.sourcePath + &quot;CELLSJAVA40944_1.xlsx&quot;);

            //Define the second source book. 
            //Open the second excel file. 
            Workbook SourceBook2 = new Workbook(Constants.sourcePath + &quot;CELLSJAVA40944_2.xlsx&quot;);

            //Combining the two workbooks 
            SourceBook1.Combine(SourceBook2);
            SourceBook2.Worksheets.ActiveSheetIndex = 1;
            SourceBook1.Worksheets[1].Cells[&quot;A1&quot;].PutValue(&quot;Click the ole object.&quot;);

           Util.SaveManCheck(SourceBook1, &quot;Shape&quot;, &quot;CELLSJAVA40944.xlsx&quot;);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


