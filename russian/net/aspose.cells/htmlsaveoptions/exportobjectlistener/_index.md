---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задает ExportObjectListener для экспорта объектов"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Получает или задает ExportObjectListener для экспорта объектов.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство HtmlSaveOptions.IStreamProvider. Это свойство будет удалено через 12 месяцев, начиная с августа 2015 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // Создайте пользовательский слушатель экспорта объектов
            var listener = new CustomExportObjectListener();
            
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Создайте параметры сохранения HTML с этим слушателем
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // Сохраните в файл HTML
            workbook.Save("output.html", saveOptions);
        }
    }

    // Пользовательская реализация IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Пример: Обработайте экспортированный объект
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Верните исходный объект (можно изменить его при необходимости)
            return e;
        }
    }
}
```

### См. также

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


