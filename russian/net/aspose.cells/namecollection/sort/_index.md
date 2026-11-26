---
title: "NameCollection.Sort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NameCollection. Сортирует определённые имена"
type: docs
url: /ru/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Сортирует определённые имена.

```csharp
public void Sort()
```

### Примечания

Если вы создаёте большое количество именованных диапазонов в файле Excel, пожалуйста, вызовите этот метод после создания всех именованных диапазонов и перед сохранением.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите NameCollection из книги
            NameCollection names = workbook.Worksheets.Names;
            
            // Добавьте несколько именованных диапазонов для демонстрации сортировки
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Отобразить имена до сортировки
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Вызовите метод Sort
                names.Sort();
                
                // Отобразить имена после сортировки
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### См. также

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


