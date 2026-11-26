---
title: "Перечисление SensitivityLabelMarkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Представляет типы маркировки контента, которые следует применять к файлу"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Представляет типы маркировки контента, которые должны применяться к файлу.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет |
| Header | `1` | Заголовок |
| Footer | `2` | Нижний колонтитул |
| Watermark | `4` | Водяной знак |
| Encryption | `8` | Шифрование |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelMarkTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрировать значения перечисления SensitivityLabelMarkType
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Применить различные маркировки метки конфиденциальности в зависимости от типа
            switch (markType)
            {
                case SensitivityLabelMarkType.None:
                    Console.WriteLine("No sensitivity label applied");
                    break;
                case SensitivityLabelMarkType.Header:
                    worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
                    break;
                case SensitivityLabelMarkType.Footer:
                    worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
                    break;
                case SensitivityLabelMarkType.Watermark:
                    worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
                    break;
                case SensitivityLabelMarkType.Encryption:
                    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
                    break;
            }

            // Сохранить книгу с применённой меткой конфиденциальности
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


