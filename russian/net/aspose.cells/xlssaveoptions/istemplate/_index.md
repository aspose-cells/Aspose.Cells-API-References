---
title: "XlsSaveOptions.IsTemplate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XlsSaveOptions. Указывает, сохраняется ли файл как шаблон"
type: docs
url: /ru/net/aspose.cells/xlssaveoptions/istemplate/
---
## XlsSaveOptions.IsTemplate property

Указывает, сохраняется ли файл как шаблон.

```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, создайте XlsSaveOptions с соответствующим форматом сохранения (xlt для true и xls для false). Этот метод будет удалён через 12 месяцев, начиная с августа 2020 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyIsTemplateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные в первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Template");
            
            // Сохранить как файл шаблона
            string outputPath = "output_template.xlt";
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.IsTemplate = true;
            
            using (FileStream fs = File.Create(outputPath))
            {
                workbook.Save(fs, saveOptions);
            }
            
            // Проверьте формат сохранённого файла
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("File format: " + loadedWorkbook.FileFormat);
        }
    }
}
```

### См. также

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


