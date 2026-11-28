---
title: "Validation.Value1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Veri doğrulamasıyla ilişkili ilk değeri temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Veri doğrulama ile ilişkili ilk değeri temsil eder.

```csharp
public object Value1 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresinde bir doğrulama oluşturun
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Value1 özelliğini dize dizisiyle ayarlayın
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Doğrulama değerlerini alın ve görüntüleyin
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // B1 hücresinde farklı değerlerle başka bir doğrulama oluşturun
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // İkinci doğrulama değerlerini alın ve görüntüleyin
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


