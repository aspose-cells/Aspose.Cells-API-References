---
title: "Перечисление OoxmlCompressionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.OoxmlCompressionType. Тип сжатия Ooxml"
type: docs
url: /ru/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

Тип сжатия Ooxml

```csharp
public enum OoxmlCompressionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Level1 | `1` | Самое быстрое, но наименее эффективное сжатие. |
| Level2 | `2` | Немного медленнее, но лучше, чем уровень 1. |
| Level3 | `3` | Немного медленнее, но лучше, чем уровень 2. |
| Level4 | `4` | Немного медленнее, но лучше, чем уровень 3. |
| Level5 | `5` | Немного медленнее, чем уровень 4, но с лучшим сжатием. |
| Level6 | `6` | Хороший баланс скорости и эффективности сжатия. |
| Level7 | `7` | Довольно хорошее сжатие! |
| Level8 | `8` | Лучшее сжатие, чем Level7! |
| Level9 | `9` | «Лучшее» сжатие, где лучше означает наибольшее уменьшение размера входного потока данных. Это также самое медленное сжатие. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Создать OoxmlSaveOptions и установить тип сжатия
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Сохранить книгу с указанным типом сжатия
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


