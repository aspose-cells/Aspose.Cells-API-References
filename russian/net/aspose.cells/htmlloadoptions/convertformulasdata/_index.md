---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlLoadOptions. Если true, преобразует строку в формулу, когда значение строки начинается с символа; значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

Если true, преобразует строку в формулу, когда значение строки начинается с символа '=', значение по умолчанию — false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство HtmlLoadOptions.HasFormula. Это свойство будет удалено через 12 месяцев, начиная с марта 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // Создать экземпляр HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Установите свойство ConvertFormulasData в true
            options.ConvertFormulasData = true;

            // Загрузить HTML‑файл в книгу Workbook, используя указанные параметры
            Workbook workbook = new Workbook("input.html", options);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразить некоторые значения ячеек, чтобы продемонстрировать преобразование формул
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // Сохраните Workbook в файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


