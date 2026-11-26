---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор XpsSaveOptions. Создаёт параметры для сохранения файла xps"
type: docs
url: /ru/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Создаёт параметры для сохранения файла xps.

```csharp
public XpsSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Инициализировать XpsSaveOptions с помощью конструктора
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Настроить параметры сохранения
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Сохранить книгу с параметрами
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### См. также

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Создаёт параметры для сохранения файла xps.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат сохранения, он должен быть в формате xps. |

### Примечания

ПРИМЕЧАНИЕ: Этот конструктор теперь устарел. Вместо этого, пожалуйста, используйте конструктор XpsSaveOptions(). Это свойство будет удалено через 12 месяцев, начиная с августа 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // Создайте XpsSaveOptions, используя конструктор с параметром SaveFormat.
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // Сохранить книгу с указанными параметрами
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


