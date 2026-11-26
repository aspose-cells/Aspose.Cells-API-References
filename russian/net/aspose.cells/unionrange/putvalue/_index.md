---
title: "UnionRange.PutValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Помещает значение в диапазон; при необходимости значение будет преобразовано к другому типу данных, а числовой формат ячеек будет сброшен"
type: docs
url: /ru/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | String | Входное значение |
| isConverted | Boolean | True: преобразовано в другой тип данных, если это уместно. |
| setStyle | Boolean | True: установить числовой формат в стиль ячейки при преобразовании в другой тип данных |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте объединённый диапазон, охватывающий ячейки A1 до B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // Вызовите PutValue с параметрами: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Отобразите информацию о диапазоне, чтобы показать эффект
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Примените форматирование, чтобы эффект был видим
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


