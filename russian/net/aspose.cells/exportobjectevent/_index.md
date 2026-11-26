---
title: "Класс ExportObjectEvent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExportObjectEvent. Событие, вызываемое при экспорте объекта, например изображения"
type: docs
url: /ru/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

Событие, вызываемое при экспорте объекта, например Picture.

```csharp
public class ExportObjectEvent
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Получает объект для экспорта. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventDemo
    {
        public static void ExportObjectEventExample()
        {
            // Пользовательская реализация IExportObjectListener
            // Сохранить HTML‑файл с пользовательским слушателем
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;

        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape shape)
            {
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }

        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Здесь сохраняйте изображение в любое место, затем возвращайте URL (относительный или абсолютный), по которому сгенерированный HTML может получить изображение
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


