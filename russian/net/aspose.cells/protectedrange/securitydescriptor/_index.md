---
title: "ProtectedRange.SecurityDescriptor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ProtectedRange. Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без предоставления пароля для доступа к диапазону"
type: docs
url: /ru/net/aspose.cells/protectedrange/securitydescriptor/
---
## ProtectedRange.SecurityDescriptor property

Селектор безопасности определяет учётные записи пользователей, которые могут редактировать этот диапазон без ввода пароля для доступа к диапазону.

```csharp
public string SecurityDescriptor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertySecurityDescriptorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            ProtectedRange r = pranges[index];
            
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            r.SecurityDescriptor = securityDescriptor;
            
            string outputPath = "ProtectedRangeWithSecurityDescriptor.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with protected range security descriptor: " + outputPath);
        }
    }
}
```

### См. также

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


