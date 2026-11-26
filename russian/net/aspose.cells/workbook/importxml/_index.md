---
title: "Workbook.ImportXml"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Импортирует/Обновляет XML‑файл данных в книгу"
type: docs
url: /ru/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Импортирует/обновляет XML-файл данных в рабочую книгу.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| url | String | url/путь к xml‑файлу. |
| sheetName | String | имя листа назначения. |
| строка | Int32 | строка назначения |
| col | Int32 | столбец назначения |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Создать объект рабочей книги
            Workbook wb = new Workbook();
            
            // Импортировать XML‑данные в первый лист, начиная с ячейки A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Импортирует/обновляет XML-файл данных в рабочую книгу.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | поток XML‑файла. |
| sheetName | String | имя листа назначения. |
| строка | Int32 | строка назначения. |
| col | Int32 | столбец назначения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodImportXmlWithStreamStringInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать пример XML‑данных
            string xmlData = @"<Products>
                <Product>
                    <Name>Laptop</Name>
                    <Price>999.99</Price>
                </Product>
                <Product>
                    <Name>Phone</Name>
                    <Price>699.99</Price>
                </Product>
            </Products>";

            // Преобразовать строку XML в MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // Импортировать XML‑данные в книгу, начиная с ячейки A1 первого листа
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Сохраните книгу
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Очистить ресурсы
                xmlStream.Dispose();
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


