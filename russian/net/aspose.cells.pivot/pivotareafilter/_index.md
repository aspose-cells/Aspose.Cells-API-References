---
title: "Класс PivotAreaFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotAreaFilter. Представляет фильтр PivotArea для PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

Представляет фильтр [`PivotArea`](../pivotarea/) для [`PivotTable`](../pivottable/).

```csharp
public class PivotAreaFilter
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Получает индекс поля в исходных полях, к которому относится этот фильтр. Значение -2 указывает на поле значений. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Указывает, имеет ли это поле выделение. Работает только когда PivotTable находится в режиме Outline. |

## Методы

| Имя | Описание |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Получает, какой подытог установлен для этого фильтра. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Подытог для фильтра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Настройка примерных данных
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // Создать PivotTable — исправить обработку возвращаемого значения
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Создать и настроить PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Продемонстрировать методы
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


