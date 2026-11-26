---
title: "Worksheet.Protect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Защищает лист"
type: docs
url: /ru/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Защищает лист.

```csharp
public void Protect(ProtectionType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ProtectionType | Тип защиты. |

### Примечания

Этот метод защищает лист без пароля. Он может защищать лист во всех версиях файлов Excel.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Защитить лист типом защиты Objects
            sheet.Protect(ProtectionType.Objects);
            
            // Сохраните книгу
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### См. также

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Защищает лист.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ProtectionType | Тип защиты. |
| пароль | String | Пароль. |
| oldPassword | String | Если лист уже защищён паролем, пожалуйста, укажите старый пароль. В противном случае вы можете установить значение null или пустую строку для этого параметра. |

### Примечания

Этот метод может защищать лист в любых версиях файла Excel.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Защитите лист паролем и разрешите все типы защиты
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Сохраните книгу
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### См. также

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


