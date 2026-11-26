---
title: "PivotField.GetSubtotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Указывает, следует ли показывать указанный промежуточный итог для этого поля сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Указывает, следует ли показывать указанный промежуточный итог для этого поля сводки.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Тип промежуточного итога. |

### Возвращаемое значение

Возвращает, отображается ли указанный промежуточный итог.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Проверьте, включён ли промежуточный итог Сумма
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Проверьте, включён ли промежуточный итог Среднее
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Включить промежуточный итог Сумма
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Проверьте, что промежуточный итог Сумма теперь включён
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Обновите сводную таблицу, чтобы отобразить изменения
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


