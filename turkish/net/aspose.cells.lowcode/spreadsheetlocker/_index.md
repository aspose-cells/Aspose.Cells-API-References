---
title: "Sınıf SpreadsheetLocker"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.SpreadsheetLocker sınıfı. Elektronik tablo dosyasını kilitlemek için düşük kod API'si"
type: docs
url: /tr/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

Elektronik tablo dosyasını kilitlemek için düşük kodlu API.

```csharp
public class SpreadsheetLocker
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Belirtilen ayarlarla elektronik tablo dosyasını kilitler. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // Çalışma kitabını korumak için SpreadsheetLocker'ı kullanın
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


