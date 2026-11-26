---
title: "Hyperlink.TextToDisplay"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Hyperlink. Представляет текст, отображаемый для указанной гиперссылки. Значение по умолчанию — адрес гиперссылки"
type: docs
url: /ru/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Представляет текст, отображаемый для указанной гиперссылки. Значение по умолчанию — адрес гиперссылки.

```csharp
public string TextToDisplay { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyTextToDisplayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте гиперссылки с свойством TextToDisplay
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Добавьте первую гиперссылку с пользовательским отображаемым текстом
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Добавить вторую гиперссылку с пользовательским отображаемым текстом
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Добавить третью гиперссылку с ссылкой на ячейку в качестве отображаемого текста
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Сохраните книгу
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### См. также

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


