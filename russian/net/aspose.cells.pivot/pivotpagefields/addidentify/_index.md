---
title: "PivotPageFields.AddIdentify"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotPageFields. Устанавливает, какой ярлык элемента в каждом поле страницы использовать для идентификации диапазона данных. Длина pageItemIndex должна быть равна PageFieldCount, поэтому пожалуйста сначала добавьте поле страницы."
type: docs
url: /ru/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Устанавливает, какую метку элемента в каждом поле страницы использовать для идентификации диапазона данных. Длина pageItemIndex должна быть равна PageFieldCount, поэтому сначала добавьте поле страницы.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeIndex | Int32 | Индекс диапазона данных консолидации. |
| pageItemIndex | Int32[] | Индекс элемента страницы в каждом поле страницы. pageItemIndex[2] = 1 означает, что второй элемент в третьем поле используется для идентификации этого диапазона. pageItemIndex[1] = -1 означает, что в втором поле нет элемента для идентификации этого диапазона, и MS автоматически создаст элемент \"blank\" во втором поле для идентификации этого диапазона. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Создавайте экземпляр PivotPageFields напрямую, а не получая его через PivotTable
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


