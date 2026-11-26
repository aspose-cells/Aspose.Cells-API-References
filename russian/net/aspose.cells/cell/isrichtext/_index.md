---
title: "Cell.IsRichText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Указывает, является ли строковое значение этой ячейки текстом с богатым форматированием"
type: docs
url: /ru/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Указывает, является ли строковое значение этой ячейки текстом с богатым форматированием.

```csharp
public bool IsRichText()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать ячейку с форматированием богатого текста
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Применить форматирование богатого текста
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Проверьте, содержит ли ячейка богатый текст
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Сохраните книгу
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


