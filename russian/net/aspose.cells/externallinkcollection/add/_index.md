---
title: "ExternalLinkCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExternalLinkCollection. Добавляет внешнюю ссылку"
type: docs
url: /ru/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Добавляет внешнюю ссылку.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Внешнее имя файла. |
| sheetNames | String[] | Все имена листов внешнего файла. |

### Возвращаемое значение

Позиция внешнего имени в этом списке.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить коллекцию внешних ссылок
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Подготовьте параметры для метода Add
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Вызовите метод Add с параметрами (String, String[])
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Отобразить информацию о добавленной внешней ссылке
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link file: {link.DataSource}");
                Console.WriteLine("Referenced sheets:");
                foreach (string sheet in sheetNames)
                {
                    Console.WriteLine($"- {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### См. также

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Добавить внешнюю ссылку .

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directoryType | DirectoryType | Тип каталога имени файла. |
| fileName | String | имя файла. |
| sheetNames | String[] | Все имена листов внешнего файла. |

### Возвращаемое значение

Позиция внешнего имени в этом списке.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить коллекцию внешних ссылок
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Подготовьте параметры для метода Add
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Вызовите метод Add с параметрами (DirectoryType, String, String[])
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Отобразить информацию о добавленной внешней ссылке
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link references: {link.DataSource}");
                foreach (string sheet in sheetNames) // Changed from link.SheetNames to sheetNames
                {
                    Console.WriteLine($" - References sheet: {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### См. также

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


