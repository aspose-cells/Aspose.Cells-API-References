---
title: "WorkbookMetadata.Save"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookMetadata. Сохраняет изменённые метаданные в файл"
type: docs
url: /ru/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Сохраните изменённые метаданные в файл.

```csharp
public void Save(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Создать новые метаданные книги
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Добавить пользовательские свойства
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Сохранить с указанием строкового пути
            doc.Save("output.xlsb");
            
            // Проверьте сохранённый файл
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### См. также

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Сохраните изменённые метаданные в поток.

```csharp
public void Save(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSaveWithStreamDemo
    {
        public static void Run()
        {
            try
            {
                // Путь к существующей книге (убедитесь, что файл существует в папке выполнения)
                string sourcePath = "Sample.xlsx";

                // Создать MetadataOptions для свойств документа
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Создать экземпляр WorkbookMetadata с исходным файлом и параметрами
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Получить доступ к встроенной коллекции свойств документа (только для чтения)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Сохранить метаданные в новый файл с использованием потока
                using (FileStream outputStream = new FileStream("MetadataOutput.xlsx",
                                                              FileMode.Create,
                                                              FileAccess.Write))
                {
                    metadata.Save(outputStream);
                }

                Console.WriteLine("Metadata saved successfully to stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during metadata Save: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


