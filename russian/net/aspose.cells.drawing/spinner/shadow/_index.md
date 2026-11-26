---
title: "Spinner.Shadow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Spinner. Указывает, имеет ли элемент 3D-тень"
type: docs
url: /ru/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Указывает, имеет ли фигура 3‑D затенение.

```csharp
public bool Shadow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте Spinner в лист
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Установите свойства Spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Продемонстрировать свойство Shadow
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Сохраните книгу
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Загрузить сохранённую книгу, чтобы проверить свойство тени
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### См. также

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


