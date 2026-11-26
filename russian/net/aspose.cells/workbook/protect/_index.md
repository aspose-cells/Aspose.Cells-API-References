---
title: "Workbook.Protect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Защищает книгу"
type: docs
url: /ru/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Защищает книгу.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| protectionType | ProtectionType | Тип защиты. |
| пароль | String | Пароль для защиты книги. |

### Примеры

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

### См. также

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


