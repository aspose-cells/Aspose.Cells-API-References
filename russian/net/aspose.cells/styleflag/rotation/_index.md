---
title: "StyleFlag.Rotation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка Rotation будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Настройка вращения будет применена.

```csharp
public bool Rotation { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Получить стиль ячейки
            Style style = workbook.CreateStyle();

            // Установить новое значение вращения (45 градусов)
            style.RotationAngle = 45;

            // Отобразить текущее значение вращения
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Создать флаг стиля и включить флаг вращения
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Применить стиль с вращением к ячейке
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Сохранить результат
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


