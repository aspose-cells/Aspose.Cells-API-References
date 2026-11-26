---
title: "CellsHelper.GetCacheFolder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает папку для временных файлов, которые могут использоваться в качестве кэша данных"
type: docs
url: /ru/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Получает папку для временных файлов, которые могут использоваться в качестве кэша данных.

```csharp
public static string GetCacheFolder()
```

### Возвращаемое значение

Папка для файлов кэша, которая была указана. Если она не указана, будет возвращено null, и при необходимости будет использован системный временный путь.

### Примечания

Файлы кэша обычно используются для некоторых функций, связанных с производительностью памяти, например при сохранении большого набора данных в файл xls или при использовании режима памяти с файловым кэшем для модели ячеек.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetCacheFolderDemo
    {
        public static void Run()
        {
            try
            {
                // Получить текущий путь к папке кэша
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Отобразить путь к папке кэша
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // При необходимости установите новую папку кэша (демонстрируя соответствующий метод)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Проверьте изменение
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Вернуться к оригиналу (необязательно)
                CellsHelper.SetCacheFolder(cacheFolder);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with cache folder: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


