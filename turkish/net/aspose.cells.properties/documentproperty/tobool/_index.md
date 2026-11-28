---
title: "DocumentProperty.ToBool"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty yöntemi. Özellik değerini bool olarak döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Özellik değerini bool olarak döndürür.

```csharp
public bool ToBool()
```

### Açıklamalar

Özellik türü PropertyType.Boolean değilse bir istisna fırlatır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Boolean bir özel belge özelliği ekleyin
            customProperties.Add("IsApproved", true);
            
            // Özelliği alın ve ToBool() kullanarak bool'a dönüştürün
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


