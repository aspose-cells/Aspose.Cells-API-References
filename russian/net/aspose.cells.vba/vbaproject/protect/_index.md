---
title: "VbaProject.Protect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProject. Защищает или снимает защиту с этого VBA проекта"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Защищает или снимает защиту с этого проекта VBA.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| islockedForViewing | Boolean | Указывает, блокирует ли проект просмотр. |
| пароль | String | Если значение равно null, снимает защиту с этого VBA проекта, иначе защищает этот VBA проект. |

### Примечания

Если islockedForViewing равно true, пароль не может быть null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // Создайте книгу с проектом VBA
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Сохраните книгу
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


