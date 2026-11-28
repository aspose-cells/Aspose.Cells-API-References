---
title: "Workbook.Unprotect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bir çalışma kitabının korumasını kaldırır"
type: docs
url: /tr/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Bir çalışma kitabının korumasını kaldırır.

```csharp
public void Unprotect(string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parola | String | Çalışma kitabının korumasını kaldırmak için parola. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Koruma ile bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Doğru parola ile çalışma kitabının korumasını kaldırın
            workbook.Unprotect("book");

            // Korumasız çalışma kitabını kaydedin
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


