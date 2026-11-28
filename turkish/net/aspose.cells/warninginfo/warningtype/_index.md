---
title: "WarningInfo.WarningType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WarningInfo özelliği. Uyarı tipini alın."
type: docs
url: /tr/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Uyarı türünü al.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WarningInfo.Type özelliğini kullanın. Bu özellik, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve bir uyarı tetikleyin.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Desteklenmeyen özelliklerle kaydedildiğinde bir uyarı tetiklenecektir.
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Uyarılara neden olabilecek bir formatta kaydedin.
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // WarningType özelliğinin kullanımını gösterin.
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Belirli uyarı tiplerini ele alın.
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


