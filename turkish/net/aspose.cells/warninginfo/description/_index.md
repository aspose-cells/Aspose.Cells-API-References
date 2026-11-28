---
title: "WarningInfo.Description"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WarningInfo özelliği. Uyarı bilgisinin açıklamasını alın."
type: docs
url: /tr/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Uyarı bilgisinin açıklamasını al.

```csharp
public string Description { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyDescriptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Uyarıyı tetiklemek için yinelenen tanımlı bir ad oluşturun.
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // Uyarı geri çağrısını alın.
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // Uyarıyı tetiklemek için kaydedin.
            workbook.Save("output.xlsx");

            // Description özelliğinin kullanımını gösterin.
            if (callback.LastWarning != null)
            {
                Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
                Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
            }
        }
    }

    public class WarningCallback : IWarningCallback
    {
        public WarningInfo LastWarning { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            LastWarning = warningInfo;
        }
    }
}
```

### Ayrıca Bakınız

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


