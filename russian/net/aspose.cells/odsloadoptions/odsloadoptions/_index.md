---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор OdsLoadOptions. Представляет параметры загрузки ODS файла"
type: docs
url: /ru/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Представляет параметры загрузки ODS‑файла.

```csharp
public OdsLoadOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте OdsLoadOptions, используя конструктор
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Установите стиль гиперссылки, чтобы использовать значения по умолчанию Excel
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // Загрузите ODS‑файл с параметрами загрузки
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // Сохранить как XLSX
            workbook.Save("output.xlsx");
            
            // Проверьте, что стиль гиперссылки был применён
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### См. также

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Представляет параметры загрузки ODS‑файла.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | LoadFormat | Тип формата загрузки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Создайте пример ODS‑файла, если он не существует
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // Создайте OdsLoadOptions с параметром LoadFormat
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Загрузите книгу с созданными параметрами загрузки
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Сохраните, чтобы продемонстрировать успешную загрузку
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


