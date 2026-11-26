---
title: "Name.FullText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Name. Получает полный текст имени объекта с настройкой области"
type: docs
url: /ru/net/aspose.cells/name/fulltext/
---
## Name.FullText property

Получает полный текст имени объекта с настройкой области.

```csharp
public string FullText { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyFullTextDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать несколько именованных диапазонов
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells.CreateRange("A1", "B5").Name = "TestRange1";
            worksheet.Cells.CreateRange("C1", "D5").Name = "TestRange2";
            
            // Получить коллекцию имен
            NameCollection names = workbook.Worksheets.Names;
            
            // Найти имя по его FullText
            string reference = "=Sheet1!$A$1:$B$5";
            Name foundName = FindNameByFullText(names, reference);
            
            // Вывести результаты
            if (foundName != null)
            {
                Console.WriteLine("Found name: " + foundName.Text);
                Console.WriteLine("FullText: " + foundName.FullText);
            }
            else
            {
                Console.WriteLine("Name not found");
            }
        }
        
        public static Name FindNameByFullText(NameCollection names, string reference)
        {
            if (reference.IndexOf('=') == 0)
            {
                reference = reference.Substring(1);
            }
            foreach (Name nm in names)
            {
                if (nm.FullText.Equals(reference))
                {
                    return nm;
                }
            }
            return null;
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


