---
title: "XlsSaveOptions.XlsSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор XlsSaveOptions. Создаёт параметры для сохранения файла Excel 972003 xls"
type: docs
url: /ru/net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Создаёт параметры для сохранения файла Excel 97‑2003 xls.

```csharp
public XlsSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Sample XLS File");
            worksheet.Cells["A2"].PutValue("Created using XlsSaveOptions");

            // Инициализируйте XlsSaveOptions с помощью конструктора
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Установите некоторые параметры (удалены неподдерживаемые свойства)
            saveOptions.IsTemplate = false;

            // Сохраните книгу с указанными параметрами
            workbook.Save("output.xls", saveOptions);

            Console.WriteLine("File saved successfully with XlsSaveOptions.");
        }
    }
}
```

### См. также

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Создаёт параметры для сохранения файла Excel 97‑2003 xls/xlt.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат файла. Он должен быть Excel97To2003 или Xlt, иначе сохранённый формат будет автоматически установлен как Excel97To2003. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
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
                XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
                
                // Установить дополнительные свойства
                saveOptions.MatchColor = true;
                saveOptions.WpsCompatibility = false;
                
                Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
                
                // Сохранить книгу с указанными параметрами
                workbook.Save("XlsSaveOptionsCtorDemo.xls", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XlsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


