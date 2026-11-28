---
title: "VbaProject.IslockedForViewing"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir.

```csharp
[Obsolete("Use VbaProject.IsLockedForView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IslockedForViewing { get; }
```

### Açıklamalar

NOTE: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen VbaProject.IsLockedForView özelliğini kullanın. Bu özellik Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIslockedForViewingDemo
    {
        public static void Run()
        {
            // VBA projesi içeren örnek bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            // VBA projesinin oluşturulmasını sağlamak için yeni bir çalışma sayfası oluşturun
            wb.Worksheets.Add();
            
            // IslockedForViewing özelliğini gösterin
            Console.WriteLine("Initial state:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Görünüm için koruyun ve kilitleyin
            wb.VbaProject.Protect(true, "password123");
            Console.WriteLine("After protecting and locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Görünüm için kilitlemeden koruyun
            wb.VbaProject.Protect(false, "password456");
            Console.WriteLine("After protecting without locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Korumayı kaldırın
            wb.VbaProject.Protect(true, "");
            Console.WriteLine("After removing protection:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


