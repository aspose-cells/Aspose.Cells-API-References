---
title: "IExportObjectListener.ExportObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IExportObjectListener. Экспортировать один объект"
type: docs
url: /ru/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Экспортировать один объект.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| e | ExportObjectEvent | Событие, вызываемое, когда требуется экспортировать объект. |

### Возвращаемое значение

Информация о результате экспорта объекта. При экспорте объектов при сохранении рабочей книги в формате HTML результатом является строка URL для доступа к сохранённому изображению из HTML‑файла, содержащего этот экспортированный объект.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Создать экземпляр демонстрационного класса, реализующего IExportObjectListener
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // В реальном сценарии событие ExportObjectEvent будет предоставлено фреймворком
                // Для демонстрационных целей мы просто вызовем метод с null
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // Пользовательская реализация для обработки экспорта
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Вернуть изменённый объект или null, чтобы использовать поведение экспорта по умолчанию
            return null;
        }
    }
}
```

### См. также

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


