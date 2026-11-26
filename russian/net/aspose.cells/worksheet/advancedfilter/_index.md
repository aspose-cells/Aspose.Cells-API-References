---
title: "Worksheet.AdvancedFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Фильтрует данные с использованием сложных критериев"
type: docs
url: /ru/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Фильтрует данные, используя сложные критерии.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isFilter | Boolean | Указывает, осуществляется ли фильтрация списка на месте. |
| listRange | String | Диапазон списка. |
| criteriaRange | String | Диапазон критериев. |
| copyTo | String | Диапазон, в который копируются данные. |
| uniqueRecordOnly | Boolean | Только отображение или копирование уникальных строк. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для фильтрации
            // Заголовки
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Критерии
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Данные
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Применить расширенный фильтр (фильтрация на месте, только уникальные записи)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Сохраните книгу
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


