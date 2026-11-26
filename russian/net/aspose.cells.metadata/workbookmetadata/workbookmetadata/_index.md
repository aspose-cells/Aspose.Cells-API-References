---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор WorkbookMetadata. Создать объект метаданных"
type: docs
url: /ru/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

Создайте объект метаданных.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String |  |
| опции | MetadataOptions |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodCtorWithStringMetadataOptionsDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xls";
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);
            
            Console.WriteLine("WorkbookMetadata created successfully with document properties metadata.");
        }
    }
}
```

### См. также

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

Создайте объект метаданных.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream |  |
| опции | MetadataOptions |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSharpctorWithStreamMetadataOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Создать простую рабочую книгу в памяти
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // Сохранить рабочую книгу в поток памяти
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // Создать MetadataOptions (используя свойства документа в качестве примера)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- Демонстрация конструктора #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // Получить доступ к встроенной коллекции свойств документа (только для чтения)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // Сохранить метаданные в новый файл (по желанию)
                    metadata.Save("MetadataFromStream.xlsx");
                }

                Console.WriteLine("WorkbookMetadata created and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during WorkbookMetadata #ctor demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


