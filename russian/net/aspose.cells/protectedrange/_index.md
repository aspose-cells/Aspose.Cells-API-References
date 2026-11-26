---
title: "Класс ProtectedRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ProtectedRange. Указанный диапазон, который разрешено редактировать, когда защита листа включена"
type: docs
url: /ru/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Указанный диапазон, разрешённый для редактирования, когда защита листа ВКЛЮЧЕНА.

```csharp
public class ProtectedRange
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Получает объект [`CellArea`](./cellarea/), представляющий область ячеек, которую нужно защитить. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Указывает, защищён ли лист паролем. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Получает заголовок диапазона. Он используется как дескриптор, а не как определение именованного диапазона. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Представляет пароль для защиты диапазона. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | Селектор безопасности определяет учётные записи пользователей, которые могут редактировать этот диапазон без ввода пароля для доступа к диапазону. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Добавляет ссылочную область к этому |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Получает все ссылочные области. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить коллекцию защищённых диапазонов
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Добавить новый защищённый диапазон (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Получить защищённый диапазон
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Установить дескриптор безопасности
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Сохраните книгу
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


