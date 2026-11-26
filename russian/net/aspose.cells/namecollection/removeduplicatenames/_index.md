---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NameCollection. Удалить дублирующие определённые имена"
type: docs
url: /ru/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Удалить дублирующиеся определённые имена

```csharp
public void RemoveDuplicateNames()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте несколько именованных диапазонов с дублирующими именами
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Создайте дублирующие именованные диапазоны, используя правильную сигнатуру метода Add
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Отобразить количество перед удалением дубликатов
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Удалить дублирующие имена
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Отобразить количество после удаления дубликатов
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### См. также

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


