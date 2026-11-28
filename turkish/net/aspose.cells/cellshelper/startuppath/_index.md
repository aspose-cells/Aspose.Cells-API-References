---
title: "CellsHelper.StartupPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Bazı dış formül referansları tarafından başvuru yapılan başlangıç yolunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Bazı dış formül referansları tarafından kullanılan başlangıç yolunu alır veya ayarlar.

```csharp
public static string StartupPath { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Başlangıç yolunu ayarla
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Başlangıç yolunu göster
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Ek CellsHelper özelliklerini göster
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


