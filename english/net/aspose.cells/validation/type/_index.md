---
title: Validation.Type
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the data validation type
type: docs
url: /net/aspose.cells/validation/type/
---
## Validation.Type property

Represents the data validation type.

```csharp
public ValidationType Type { get; set; }
```

### Examples

```csharp
// Called: if(validation.Type == ValidationType.Date)
[Test]
       public void Property_Type()
       {
           Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA40382.xlsx&quot;);
             WorksheetCollection sheets = workbook.Worksheets;
        Worksheet sheet = sheets[0];
        ValidationCollection validations = sheet.Validations;
        
        for(int i = 0; i &lt; validations.Count; i++){
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

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


