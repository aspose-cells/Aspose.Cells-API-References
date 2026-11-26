---
title: "Перечисление OoxmlCompliance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.OoxmlCompliance. Позволяет указать, какая спецификация OOXML будет использоваться при сохранении в формате Xlsx"
type: docs
url: /ru/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Позволяет указать, какая спецификация OOXML будет использоваться при сохранении в формате Xlsx.

```csharp
public enum OoxmlCompliance
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1-е издание, 2006. |
| Iso29500_2008_Strict | `1` | Уровень строгого соответствия ISO/IEC 29500:2008. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установить уровень соответствия OOXML на ISO/IEC 29500:2008 Strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Добавить некоторые данные в лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Сохранить рабочую книгу с указанным уровнем соответствия OOXML
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


