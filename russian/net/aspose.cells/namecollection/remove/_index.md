---
title: "NameCollection.Remove"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NameCollection. Удалить массив имён"
type: docs
url: /ru/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Удалить массив имён

```csharp
public void Remove(string[] names)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| имена | String[] | Текст имён. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите NameCollection из книги
            NameCollection names = workbook.Worksheets.Names;
            
            // Добавьте несколько именованных диапазонов, чтобы продемонстрировать удаление
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Подготовьте массив имён для удаления
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Вызовите метод Remove с параметром String[]
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Отобразить оставшиеся имена
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### См. также

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Удалить имя.

```csharp
public void Remove(string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Текст имени. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить именованный диапазон
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Отобразить количество перед удалением
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Удалить именованный диапазон
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Отобразить количество после удаления
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### См. также

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


