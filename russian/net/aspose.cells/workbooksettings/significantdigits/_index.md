---
title: "WorkbookSettings.SignificantDigits"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Возвращает и задаёт количество значимых цифр. Значение по умолчанию — SignificantDigits"
type: docs
url: /ru/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Возвращает и задаёт количество значимых цифр. Значение по умолчанию — [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Примечания

Сейчас может быть только 15 или 17. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [`SignificantDigitsType`](../significantdigitstype/). Это свойство будет удалено через 12 месяцев, начиная с июня 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте пример числовых данных для демонстрации значимых цифр
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Установите значимые цифры в 15 (максимальная точность для double)
            settings.SignificantDigits = 15;

            // Сохраните книгу, чтобы показать эффект значимых цифр
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


