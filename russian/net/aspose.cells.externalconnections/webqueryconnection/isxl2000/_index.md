---
title: "WebQueryConnection.IsXl2000"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Этот флаг существует для обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб‑запрос был обновлён в приложении для электронных таблиц версии Microsoft Excel 2000 или новее. Это необязательный атрибут, который можно игнорировать"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Этот флаг существует для обеспечения обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб‑запрос был обновлён в приложении электронных таблиц, версии не ниже Microsoft Excel 2000. Это необязательный атрибут, который можно игнорировать.

```csharp
public bool IsXl2000 { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите первое существующее подключение веб‑запроса (если есть)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразите начальное значение IsXl2000
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Установите IsXl2000 в true (поскольку он доступен для чтения и записи)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Установите IsXl2000 обратно в false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


