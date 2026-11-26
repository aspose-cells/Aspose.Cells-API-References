---
title: "Класс WarningInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WarningInfo. Информация о предупреждении"
type: docs
url: /ru/net/aspose.cells/warninginfo/
---
## WarningInfo class

Информация о предупреждении

```csharp
public class WarningInfo
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Получает и задает исправленный объект. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Получить описание информации о предупреждении. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | Объект ошибки. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Получить тип предупреждения. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Получить тип предупреждения. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassWarningInfoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить обратный вызов предупреждения
            workbook.Settings.WarningCallback = new WarningHandler();

            // Вызвать разные типы предупреждений
            worksheet.Cells["A1"].PutValue("InvalidName"); // Will trigger DefinedName warning
            worksheet.Cells["A2"].PutValue(DateTime.MaxValue); // May trigger other warnings

            Console.WriteLine("Warning demo completed.");
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            switch (warningInfo.WarningType)
            {
                case WarningType.DuplicateDefinedName:
                    warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                    Console.WriteLine($"DefinedName warning handled. Corrected to: {warningInfo.CorrectedObject}");
                    break;
                case WarningType.FontSubstitution:
                    Console.WriteLine($"Font warning: {warningInfo.Description}");
                    break;
                case WarningType.UnsupportedFileFormat:
                    Console.WriteLine($"File format warning: {warningInfo.Description}");
                    break;
                case WarningType.IO:
                    Console.WriteLine($"IO warning: {warningInfo.Description}");
                    break;
                case WarningType.InvalidData:
                case WarningType.Limitation:
                    Console.WriteLine($"Warning: {warningInfo.Description}");
                    break;
                default:
                    Console.WriteLine($"Unknown warning type: {warningInfo.Description}");
                    break;
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


