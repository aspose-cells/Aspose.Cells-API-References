---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OoxmlSaveOptions. Указывает, следует ли обновлять коэффициент масштабирования перед сохранением файла, если свойства PageSetup.FitToPagesWide и PageSetup.FitToPagesTall управляют масштабированием листа"
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Указывает, следует ли обновлять коэффициент масштабирования перед сохранением файла, если свойства PageSetup.FitToPagesWide и PageSetup.FitToPagesTall контролируют масштабирование листа.

```csharp
public bool UpdateZoom { get; set; }
```

### Примечания

Значение по умолчанию — false для повышения производительности.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyUpdateZoomDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите начальный уровень масштабирования
            worksheet.PageSetup.Zoom = 100;

            // Создайте параметры сохранения с включённым UpdateZoom
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // Сохранить в поток памяти
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Перезагрузите книгу, чтобы проверить, что масштаб был обновлён
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### См. также

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


