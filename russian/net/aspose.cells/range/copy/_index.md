---
title: "Range.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Копирование диапазона с параметрами специальной вставки"
type: docs
url: /ru/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Копирует диапазон с параметрами специальной вставки.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | Диапазон | Исходный диапазон. |
| опции | PasteOptions | Параметры специальной вставки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangePasteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Создать примерные данные в исходном диапазоне
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Создать диапазоны с полностью квалифицированным типом
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Установить параметры вставки
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Копировать с параметрами вставки
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Копирует данные (включая формулы), форматирование, графические объекты и т.д. из исходного диапазона.

```csharp
public void Copy(Range range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| range | Range | Исходный объект [`Range`](../). |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Создайте исходные и целевые диапазоны
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Заполнить исходный диапазон примерными данными
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Скопировать исходный диапазон в назначение
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


