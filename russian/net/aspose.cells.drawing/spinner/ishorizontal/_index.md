---
title: "Spinner.IsHorizontal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Spinner. Указывает, является ли это горизонтальной полосой прокрутки"
type: docs
url: /ru/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Указывает, является ли это горизонтальной полосой прокрутки.

```csharp
public bool IsHorizontal { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Добавить элемент управления Spinner на лист
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Установите свойства Spinner
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // Продемонстрировать свойство IsHorizontal (чтение и запись)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Переключить ориентацию
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Сохраните книгу
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


