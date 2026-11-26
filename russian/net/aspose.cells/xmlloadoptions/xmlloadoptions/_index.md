---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор XmlLoadOptions. Представляет параметры загрузки XML‑файла"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Представляет параметры загрузки xml‑файла.

```csharp
public XmlLoadOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте новые параметры загрузки XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Установите преобразование числовых или датовых значений
            options.ConvertNumericOrDate = true;
            
            // Загрузить книгу с параметрами
            Workbook workbook = new Workbook("input.xml", options);
            
            // Получите доступ к данным ячейки
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Сохранить книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Представляет параметры загрузки xml‑файла.

```csharp
public XmlLoadOptions(LoadFormat type)
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

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр XmlLoadOptions с параметром LoadFormat
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Установите некоторые свойства XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Создайте книгу, используя параметры загрузки
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];

                // Отобразите некоторую информацию
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Сохраните книгу
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


