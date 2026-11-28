---
title: "Workbook.Protect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bir çalışma kitabını korur"
type: docs
url: /tr/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Bir çalışma kitabını korur.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| protectionType | ProtectionType | Koruma türü. |
| parola | String | Çalışma kitabını korumak için şifre. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectWithProtectionTypeStringDemo
    {
        public static void Run()
        {
            Workbook wbk = new Workbook();
            wbk.Protect(ProtectionType.Structure, "password123");
            
            wbk.Save("protected_workbook.xlsx", SaveFormat.Xlsx);
            wbk.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


