---
title: "CellsHelper.AltStartPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Alternatif başlangıç yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından referans alınır."
type: docs
url: /tr/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Bazı dış formül referansları tarafından kullanılan alternatif başlangıç yolunu alır veya ayarlar.

```csharp
public static string AltStartPath { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Alternatif başlangıç yolunu ayarla
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // Demonstrasyon için diğer ilgili özellikleri de ayarla
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Özelliğin kullanımını göstermek için yolları görüntüle
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Bu yolların nasıl kullanılabileceğine örnek
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


