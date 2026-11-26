---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoNumberedBulletValue. Представляет схему автоматической нумерации"
type: docs
url: /ru/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Представляет схему автоматической нумерации.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новый экземпляр AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // Отобразить начальное значение AutonumberScheme
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Установить новое значение AutonumberScheme
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Создать книгу, чтобы продемонстрировать маркер в контексте
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Создать форму с текстом, который будет использовать стиль маркера
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Примечание: Фактическое применение стиля маркера к тексту потребует дополнительных вызовов API
                // не показано в рефлексии. Мы просто сохраним книгу в качестве демонстрации.
                workbook.Save("AutonumberSchemeDemo.xlsx");
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

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


