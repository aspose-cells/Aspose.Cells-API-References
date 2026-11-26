---
title: "Chart.ChangeTemplate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Изменить тип диаграммы с помощью предустановленного шаблона"
type: docs
url: /ru/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Изменить тип диаграммы с помощью предустановленного шаблона.

```csharp
public void ChangeTemplate(byte[] data)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| данные | Byte[] | Данные файла шаблона диаграммы (.crtx). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", false);

            // Получить данные шаблона из другого файла диаграммы
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // Вызвать метод ChangeTemplate с параметром массив байтов
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Показать эффект, сохранив рабочую книгу
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


