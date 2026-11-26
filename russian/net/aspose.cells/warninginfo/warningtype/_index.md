---
title: "WarningInfo.WarningType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WarningInfo. Получить тип предупреждения"
type: docs
url: /ru/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Получить тип предупреждения.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство WarningInfo.Type. Это свойство будет удалено через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу и вызовите предупреждение
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Это вызовет предупреждение при сохранении с неподдерживаемыми функциями
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Сохранить в формате, который может вызвать предупреждения
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Продемонстрировать использование свойства WarningType
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Обрабатывать конкретные типы предупреждений
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### См. также

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


