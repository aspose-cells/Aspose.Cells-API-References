---
title: "SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SpreadsheetML2003SaveOptions. Создаёт параметры для сохранения файла Excel 2003 в формате spreadml."
type: docs
url: /ru/net/aspose.cells/spreadsheetml2003saveoptions/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions() {#constructor}

Создаёт параметры для сохранения файла Excel 2003 в формате spreadml.

```csharp
public SpreadsheetML2003SaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и добавить примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Создайте SpreadsheetML2003SaveOptions с помощью конструктора.
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            
            // Установите параметры.
            saveOptions.LimitAsXls = true;
            saveOptions.ExportColumnIndexOfCell = true;

            // Сохраните с параметрами.
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with SpreadsheetML2003SaveOptions");
        }
    }
}
```

### См. также

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}

Создаёт параметры для сохранения файла Excel 2003 в формате spreadml.

```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат сохранения. |

### Примечания

ПРИМЕЧАНИЕ: Этот конструктор теперь устарел. Вместо него, пожалуйста, используйте конструктор SpreadsheetML2003SaveOptions(). Это свойство будет удалено через 12 месяцев, начиная с января 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);

            try
            {
                // Вызовите метод #ctor с параметром SaveFormat
                SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

                // Установите некоторые свойства параметров сохранения
                saveOptions.IsIndentedFormatting = true;
                saveOptions.LimitAsXls = false;
                saveOptions.ExportColumnIndexOfCell = true;

                Console.WriteLine("SpreadsheetML2003SaveOptions created successfully with SaveFormat parameter");

                // Сохраните книгу, используя созданные параметры сохранения.
                workbook.Save("SpreadsheetML2003Output.xml", saveOptions);
                Console.WriteLine("Workbook saved successfully with SpreadsheetML2003SaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SpreadsheetML2003SaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


