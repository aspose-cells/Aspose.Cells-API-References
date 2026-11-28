---
title: "WarningInfo sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WarningInfo sınıfı. Uyarı bilgisi"
type: docs
url: /tr/net/aspose.cells/warninginfo/
---
## WarningInfo class

Uyarı bilgisi

```csharp
public class WarningInfo
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Düzeltilen nesneyi alır ve ayarlar. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Uyarı bilgisinin açıklamasını al. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | Hata nesnesi. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Uyarı türünü al. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Uyarı türünü al. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassWarningInfoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Uyarı geri çağrısını ayarla
            workbook.Settings.WarningCallback = new WarningHandler();

            // Farklı uyarı türlerini tetikle
            worksheet.Cells["A1"].PutValue("InvalidName"); // Will trigger DefinedName warning
            worksheet.Cells["A2"].PutValue(DateTime.MaxValue); // May trigger other warnings

            Console.WriteLine("Warning demo completed.");
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            switch (warningInfo.WarningType)
            {
                case WarningType.DuplicateDefinedName:
                    warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                    Console.WriteLine($"DefinedName warning handled. Corrected to: {warningInfo.CorrectedObject}");
                    break;
                case WarningType.FontSubstitution:
                    Console.WriteLine($"Font warning: {warningInfo.Description}");
                    break;
                case WarningType.UnsupportedFileFormat:
                    Console.WriteLine($"File format warning: {warningInfo.Description}");
                    break;
                case WarningType.IO:
                    Console.WriteLine($"IO warning: {warningInfo.Description}");
                    break;
                case WarningType.InvalidData:
                case WarningType.Limitation:
                    Console.WriteLine($"Warning: {warningInfo.Description}");
                    break;
                default:
                    Console.WriteLine($"Unknown warning type: {warningInfo.Description}");
                    break;
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


