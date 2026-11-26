---
title: "ExternalLink.AddExternalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExternalLink. Добавляет внешнее имя"
type: docs
url: /ru/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Добавляет внешнее имя.

```csharp
public void AddExternalName(string text, string referTo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Текст внешнего имени. Если внешнее имя принадлежит листу, текст должен быть в виде Sheet1!Text. |
| referTo | String | Свойство referTo внешнего имени. Оно должно быть ячейкой или диапазоном. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте пример внешней рабочей книги
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Добавьте внешнюю ссылку в основную рабочую книгу
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Добавьте внешнее имя
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Используйте внешнее имя в формуле
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Вычислить формулу
            workbook.CalculateFormula();
            
            // Вывести результат.
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### См. также

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


