---
title: "SaveOptions.WarningCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Получает или задаёт обратный вызов предупреждения"
type: docs
url: /ru/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

Получает или задаёт обратный вызов предупреждения.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Создать параметры сохранения
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установить пользовательский обратный вызов предупреждения
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Это сгенерирует предупреждение о неподдерживаемой функции в формате HTML
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Сохранить с параметрами, которые могут вызвать предупреждения
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Обработать предупреждение — в данном случае просто отобразить его
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### См. также

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


