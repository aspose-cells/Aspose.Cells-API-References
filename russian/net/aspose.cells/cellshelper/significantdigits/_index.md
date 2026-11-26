---
title: "CellsHelper.SignificantDigits"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает и задает количество значимых цифр. Значение по умолчанию — 17"
type: docs
url: /ru/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Получает и задает количество значимых цифр. Значение по умолчанию — 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Примечания

Сейчас может быть только 15 или 17. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте [`SignificantDigitsType`](../significantdigitstype/). Это свойство будет удалено через 12 месяцев, начиная с июня 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Задать значимые цифры
            CellsHelper.SignificantDigits = 15;
            
            // Продемонстрировать использование свойства
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Создать книгу, чтобы продемонстрировать значимые цифры в вычислениях
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Задать значения, которые будут затронуты значимыми цифрами
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Вычислить формулы с заданными значимыми цифрами
            workbook.CalculateFormula();
            
            // Выведите результаты
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


