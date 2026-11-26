---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод HtmlTableLoadOptionCollection. Добавляет один HtmlTableLoadOption в эту коллекцию"
type: docs
url: /ru/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Добавляет один HtmlTableLoadOption в эту коллекцию.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | HtmlTableLoadOption | один HtmlTableLoadOption |

### Возвращаемое значение

индекс добавленного элемента

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод AddTableLoadOption(). Этот метод будет удалён через 6 месяцев, начиная с декабря 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Добавить параметры загрузки таблицы
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Загрузить книгу с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Сохранить вывод
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Добавьте HtmlTableLoadOption в список.

```csharp
public int Add(int tableIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tableIndex | Int32 | Индекс таблицы |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Получите доступ к экземпляру HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Добавьте новый HtmlTableLoadOption по индексу таблицы
            int index = tableLoadOptions.Add(0);

            // Получить доступ к добавленному HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Создать книгу и загрузить HTML с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Добавьте HtmlTableLoadOption в список.

```csharp
public int Add(string tableId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tableId | String | Идентификатор таблицы |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Получите доступ к экземпляру HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Добавьте новый HtmlTableLoadOption по идентификатору таблицы
            int index = tableLoadOptions.Add("mainTable");

            // Получить доступ к добавленному HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Создать книгу и загрузить HTML с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Добавьте HtmlTableLoadOption в список.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tableIndex | Int32 | Индекс таблицы |
| targetSheetIndex | Int32 | Целевой индекс листа в Excel |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать параметры загрузки HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Добавить таблицы по индексу с целевым индексом листа
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // Загрузить HTML‑файл с указанными параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Добавьте HtmlTableLoadOption в список.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tableId | String | Идентификатор таблицы |
| targetSheetIndex | Int32 | Целевой индекс листа в Excel |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Получите доступ к экземпляру HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Добавьте новый HtmlTableLoadOption по идентификатору таблицы и индексу целевого листа
            int index = tableLoadOptions.Add("tableId", 1);

            // Создать книгу и загрузить HTML с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Добавьте HtmlTableLoadOption в список.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tableIndex | Int32 | Индекс таблицы |
| targetSheetIndex | Int32 | Целевой индекс листа в Excel |
| originalSheetIndex | Int32 | Исходный индекс листа в HTML |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Создайте HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Получить доступ к HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Добавить таблицу с индексом 1, целевым индексом листа 1 и исходным индексом листа 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Создать книгу и загрузить HTML с параметрами
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Добавьте HtmlTableLoadOption в список.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tableId | String | Идентификатор таблицы |
| targetSheetIndex | Int32 | Целевой индекс листа в Excel |
| originalSheetIndex | Int32 | Исходный индекс листа в HTML |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Продемонстрировать метод Add с параметрами (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // Загрузить HTML‑файл (замените реальным путём к файлу)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


