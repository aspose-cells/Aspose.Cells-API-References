---
title: "VbaProjectReference.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReference. Получает тип этой ссылки"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Получает тип этой ссылки.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Добавить зарегистрированную ссылку в VBA проект
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Получить первую ссылку и продемонстрировать свойство Type
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Сохраните книгу
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### См. также

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


