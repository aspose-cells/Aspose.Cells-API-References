---
title: "ExternalLinkCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExternalLinkCollection. Удаляет указанную внешнюю ссылку из рабочей книги"
type: docs
url: /ru/net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Удаляет указанную внешнюю ссылку из книги.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс внешней ссылки, которую нужно удалить. |

### Примечания

При удалении внешней ссылки все формулы, которые ссылаются на неё, также будут удалены, поскольку ссылки становятся недействительными.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создайте рабочую книгу с примерными внешними ссылками
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте несколько примерных внешних ссылок
            worksheet.Cells["A1"].Formula = "='C:/ExternalFiles/File1.xlsx'!Sheet1!A1";
            worksheet.Cells["A2"].Formula = "='C:/ExternalFiles/File2.xlsx'!Sheet1!A1";
            worksheet.Cells["A3"].Formula = "='C:/ImportantFiles/File3.xlsx'!Sheet1!A1";

            // Получить коллекцию внешних ссылок
            ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Initial external links count: " + elc.Count);

            // Удалить внешние ссылки, которые не содержат "ImportantFiles" в своем пути
            for (int i = elc.Count - 1; i >= 0; i--)
            {
                if (!elc[i].DataSource.Contains("ImportantFiles"))
                {
                    elc.RemoveAt(i);
                }
            }

            Console.WriteLine("Remaining external links count: " + elc.Count);
            Console.WriteLine("Remaining external link path: " + elc[0].DataSource);
        }
    }
}
```

### См. также

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Удаляет указанную внешнюю ссылку из книги.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс внешней ссылки, которую нужно удалить. |
| updateReferencesAsLocal | Boolean | Обновлять ли все ссылки данного внешнего объекта на ссылку текущей рабочей книги. См. [`Clear`](../clear/) для получения более подробной информации об этом параметре. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            
            // Добавьте несколько внешних ссылок
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Add("externallink1.xlam", new string[] { "externallink1.xlam" });
            elc.Add("externallink2.xlam", new string[] { "externallink2.xlam" });
            elc.Add("externallink3.xlam", new string[] { "externallink3.xlam" });
            elc.Add("externallink4.xlam", new string[] { "externallink4.xlam" });

            // Добавьте несколько формул, ссылающихся на эти внешние ссылки
            Worksheet ws = wb.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    ws.Cells[j, i].Formula = $"=externallink{i+1}.xlam!customfunc{j+1}()";
                }
            }

            Console.WriteLine($"Initial external links count: {elc.Count}");
            Console.WriteLine("Formulas before removal:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Удалить по индексу 1 с updateReferences=true
            elc.RemoveAt(1, true);
            
            Console.WriteLine($"\nAfter removing at index 1 (updateReferences=true):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Updated formulas:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Удалить по индексу 0 с updateReferences=false
            elc.RemoveAt(0, false);
            
            Console.WriteLine($"\nAfter removing at index 0 (updateReferences=false):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Formulas (should be cleared where references were removed):");
            for (int i = 0; i < 2; i++)
            {
                Console.WriteLine($"Cell A{i+1}: Has formula? {ws.Cells[0, i].IsFormula}");
            }
        }
    }
}
```

### См. также

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


