---
title: "Перечисление VbaModuleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Vba.VbaModuleType. Представляет тип модуля VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

Представляет тип модуля VBA.

```csharp
public enum VbaModuleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Procedural | `0` | Представляет процедурный модуль. |
| Document | `1` | Представляет модуль документа. |
| Class | `2` | Представляет модуль класса. |
| Designer | `3` | Представляет модуль дизайнера. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавить новый модуль класса
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Получить модуль VBA
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Установить коды для модуля
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Сохраните файл Excel
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


