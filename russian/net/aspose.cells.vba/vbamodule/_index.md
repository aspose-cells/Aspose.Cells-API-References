---
title: "Класс VbaModule"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Vba.VbaModule. Представляет модуль в проекте VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Представляет модуль в проекте VBA.

```csharp
public class VbaModule
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Получает и задает бинарные коды модуля. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Получает и задает коды модуля. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Получает и задает имя модуля. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Получает тип модуля. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Добавить новый модуль
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Получить модуль VBA
            VbaModule vbaModule = vbaProject.Modules[index];

            // Установить коды для модуля
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Сохранение файла Excel
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


