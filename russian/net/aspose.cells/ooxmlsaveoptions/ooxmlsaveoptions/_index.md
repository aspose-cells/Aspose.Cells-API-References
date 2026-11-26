---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор OoxmlSaveOptions. Создаёт параметры для сохранения файла Office Open XML"
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Создаёт параметры для сохранения файла Office Open XML.

```csharp
public OoxmlSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и добавить данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Продемонстрировать конструктор OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // Сохраните книгу с параметрами OOXML
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### См. также

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Создаёт параметры для сохранения файла Office Open XML.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат файла. Он должен быть одним из следующих типов: Xlsx, Xltx, Xlam, Xlsm или Xltm, иначе сохранённый формат будет автоматически установлен как Xlsx. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // Создайте OoxmlSaveOptions с параметром SaveFormat
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Установите некоторые свойства параметров сохранения
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Сохранить книгу с указанными параметрами
                workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


