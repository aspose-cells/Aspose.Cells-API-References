---
title: "VbaProject.Protect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject yöntemi. Bu VBA projesini korur veya korumasını kaldırır"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Bu VBA projesini korur veya korumasını kaldırır.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| islockedForViewing | Boolean | projeyi görüntüleme için kilitleyip kilitlemediğini gösterir. |
| parola | String | Değer null ise, bu VBA projesinin korumasını kaldırır, aksi takdirde bu VBA projesini korur. |

### Açıklamalar

islockedForViewing true ise, şifre null olamaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // VBA projesiyle bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


