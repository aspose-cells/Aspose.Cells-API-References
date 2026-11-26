---
title: "CellsHelper.SetCacheFolder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Устанавливает папку для временных файлов, которые могут использоваться в качестве кэша данных"
type: docs
url: /ru/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Устанавливает папку для временных файлов, которые могут использоваться в качестве кэша данных.

```csharp
public static void SetCacheFolder(string cache)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| кэш | String | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |

### Примечания

Файлы кэша обычно используются для некоторых функций, связанных с производительностью памяти, например при сохранении большого набора данных в файл xls или при использовании режима памяти с файловым кэшем для модели ячеек.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodSetCacheFolderWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте временный каталог для кэша
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Установите папку кэша с помощью CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Проверьте, что папка кэша была установлена
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Создайте простой рабочий лист для демонстрации функциональности
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Сохраните книгу
                workbook.Save("CacheFolderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with cache folder configured.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting cache folder: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


