---
title: CellsHelper.GetDoubleFromDateTime
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Convert the date time to double value
type: docs
url: /net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Convert the date time to double value.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | The date time. |
| date1904 | Boolean | Date 1904 system. |

### Examples

```csharp
// Called: double d = CellsHelper.GetDoubleFromDateTime((DateTime)validation.Value1,false);
[Test]
       public void Method_Boolean_()
       {
           Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA40382.xlsx");
             WorksheetCollection sheets = workbook.Worksheets;
        Worksheet sheet = sheets[0];
        ValidationCollection validations = sheet.Validations;
        
        for(int i = 0; i < validations.Count; i++){
            Validation validation = validations[i];
            if(validation.Type == ValidationType.Date)
            {
                Assert.AreEqual(validation.Value1,new DateTime(2006,1,1));
                
               
            }else if(validation.Type == ValidationType.Time){
                double d = CellsHelper.GetDoubleFromDateTime((DateTime)validation.Value1,false);
                Assert.AreEqual(d -(int)d, 0.5);
            }
           
        }

       }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


