---
title: "Worksheet.Replace"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Заменяет весь текст ячеек новой строкой"
type: docs
url: /ru/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Заменяет весь текст ячеек новой строкой.

```csharp
public int Replace(string oldString, string newString)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| oldString | String | Значение старой строки. |
| newString | String | Значение новой строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Добавить текстовое поле с примерным текстом
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Установить верхний и нижний колонтитулы
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Заменить "Hello" на "Hi" во всем содержимом
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Заменить в заголовках/нижних колонтитулах
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Заменить в текстовых полях
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Сохраните книгу
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


