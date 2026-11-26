---
title: "NameCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NameCollection. Возвращает элемент Name по указанному индексу"
type: docs
url: /ru/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Возвращает элемент [`Name`](../../name/) по указанному индексу.

```csharp
public Name this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Получить доступ к коллекции имён
            NameCollection names = workbook.Worksheets.Names;
            
            // Добавьте именованные диапазоны, используя правильную сигнатуру метода
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Продемонстрировать использование свойства Item
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Доступ по имени с использованием свойства Item
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Изменить именованный диапазон
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### См. также

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Возвращает элемент [`Name`](../../name/) с указанным именем.

```csharp
public Name this[string text] { get; }
```

| Параметр | Описание |
| --- | --- |
| текст | Текст имени. |

### Возвращаемое значение

Элемент с указанным именем.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить коллекцию имён листов
            NameCollection names = workbook.Worksheets.Names;
            
            // Добавьте несколько именованных диапазонов (исправлено для использования правильной сигнатуры метода Add)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Получить доступ к именованным диапазонам с помощью свойства Item
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Проверьте, что имена существуют
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Попробуйте получить доступ к несуществующему имени
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### См. также

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


