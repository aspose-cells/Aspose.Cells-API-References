---
title: "ExternalLink.IsVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLink. Указывает, видна ли эта внешняя ссылка в MS Excel"
type: docs
url: /ru/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Указывает, видна ли эта внешняя ссылка в MS Excel.

```csharp
public bool IsVisible { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с внешними ссылками
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые данные в первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Создайте новую книгу, чтобы использовать её в качестве источника внешней ссылки
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Добавьте ссылку на внешнюю ссылку
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Проверьте внешние ссылки (они будут автоматически созданы при загрузке формул)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Создайте другую книгу, чтобы продемонстрировать загрузку существующего файла
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Сохраните и перезагрузите, чтобы продемонстрировать внешние ссылки
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Проверьте внешние ссылки в загруженной книге
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### См. также

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


