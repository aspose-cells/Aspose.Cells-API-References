---
title: "Перечисление EmfRenderSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.EmfRenderSetting. Параметр для рендеринга метафайла Emf"
type: docs
url: /ru/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Настройка рендеринга метафайла Emf.

```csharp
public enum EmfRenderSetting
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| EmfOnly | `0` | Только рендеринг записей Emf. |
| EmfPlusPrefer | `1` | Предпочитать рендеринг записей EmfPlus. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // Создать параметры изображения с настройкой рендеринга EMF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Создать рендер листа с этими параметрами
            SheetRender render = new SheetRender(worksheet, options);

            // Сохранить первую страницу как изображение EMF
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


