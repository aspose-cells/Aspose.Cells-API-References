---
title: "Перечисление VbaProjectReferenceType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Vba.VbaProjectReferenceType. Представляет тип ссылки на проект VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

Представляет тип ссылки проекта VBA.

```csharp
public enum VbaProjectReferenceType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Registered | `0` | Указывает ссылку на библиотеку типов Automation. |
| Control | `1` | Указывает ссылку на изменённую (twiddled) библиотеку типов и её расширенную библиотеку типов. |
| Project | `2` | Указывает ссылку на внешний проект VBA. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Добавить ссылку на проект VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Сохранение файла Excel
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Продемонстрировать использование перечисления VbaProjectReferenceType
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


