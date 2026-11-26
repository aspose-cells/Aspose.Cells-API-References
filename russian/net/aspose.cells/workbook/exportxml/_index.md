---
title: "Workbook.ExportXml"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Экспортирует XML-данные, связанные с указанной XML-картой"
type: docs
url: /ru/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Экспортировать XML-данные, связанные указанной XML-картой.

```csharp
public void ExportXml(string mapName, string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| mapName | String | имя XML-карты, которую необходимо экспортировать |
| путь | String | путь экспорта |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Создать книгу и загрузить файл Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Получить первую XmlMap из книги
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Экспортировать XML-данные, используя имя XmlMap и путь к выходному файлу
                wb.ExportXml(xmlMap.Name, "output.xml");
                Console.WriteLine("XML exported successfully to output.xml");
            }
            else
            {
                Console.WriteLine("No XmlMap found in the workbook");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Экспортировать XML-данные.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| mapName | String | имя XML-карты, которую необходимо экспортировать |
| поток | Stream | поток экспорта |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // Создать новую книгу и добавить некоторые данные
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Имя XML-карты для экспорта — для демонстрации используется заполнитель
                string mapName = "SampleMap";

                try
                {
                    // Экспортировать XML-карту в файл, используя FileStream (перегрузка String, Stream)
                    string outputPath = "ExportedSample.xml";
                    using (FileStream fs = new FileStream(outputPath, FileMode.Create, FileAccess.Write))
                    {
                        workbook.ExportXml(mapName, fs);
                    }

                    Console.WriteLine($"ExportXml completed successfully. Output saved to '{outputPath}'.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during ExportXml: {ex.Message}");
                }
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


