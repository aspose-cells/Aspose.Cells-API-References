---
title: "ExternalLink.OriginalDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLink. Представляет сохранённый источник данных внешней ссылки"
type: docs
url: /ru/net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

Представляет сохранённый источник данных внешней ссылки.

```csharp
public string OriginalDataSource { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyOriginalDataSourceDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с внешними ссылками
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить внешнюю ссылку
            worksheet.Cells["A1"].Formula = "='https://arcusventures.sharepoint.com/Fund II/[example.xlsx]Sheet1'!A1";
            
            // Изменить пути внешних ссылок
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string originalLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                string modifiedLink = originalLink.Replace(
                    @"https://arcusventures.sharepoint.com/Fund II/", 
                    @"/sites/shared/shared documents/Fund II/");
                
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = modifiedLink;
            }
            
            // Проверить изменения
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine("Modified Link: " + link.OriginalDataSource);
            }
        }
    }
}
```

### См. также

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


