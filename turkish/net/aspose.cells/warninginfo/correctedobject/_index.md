---
title: "WarningInfo.CorrectedObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WarningInfo özelliği. Düzeltlenmiş nesneyi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Düzeltilen nesneyi alır ve ayarlar.

```csharp
public object CorrectedObject { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve bir uyarı tetikleyin.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Uyarıyı normalde tetikleyecek bir ad ayarlayın
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Uyarı geri çağrısını işleyin
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Bu işlem uyarı geri çağrısını tetikleyecektir
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // CorrectedObject kullanımını gösterin
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


