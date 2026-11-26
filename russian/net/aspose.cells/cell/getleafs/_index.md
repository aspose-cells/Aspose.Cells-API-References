---
title: "Cell.GetLeafs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получить все ячейки, которые ссылаются на эту ячейку напрямую и должны быть обновлены при изменении этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Получить все ячейки, которые ссылаются на эту ячейку напрямую и должны быть обновлены при изменении этой ячейки.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Возвращаемое значение

Перечислитель для перечисления всех зависимых (Cell)

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Cell.GetDependentsInCalculation(bool), чтобы получить всех зависимых в цепочке вычислений. Это свойство будет удалено через 12 месяцев, начиная с мая 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные и формулы, чтобы создать зависимости
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Получить ячейку, у которой есть зависимые
                Cell cell = worksheet.Cells["B1"];

                // Вызовите GetLeafs, чтобы получить все ячейки, которые ссылаются на эту ячейку напрямую
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Сохраните книгу
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Получить все ячейки, которые будут обновлены при изменении этой ячейки.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| recursive | Boolean | Возвращает ли те листовые ячейки, которые не ссылаются напрямую на эту ячейку, а ссылаются на другие листовые ячейки этой ячейки |

### Возвращаемое значение

Перечислитель для перечисления всех зависимых (Cell)

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Cell.GetDependentsInCalculation(bool), чтобы получить всех зависимых в цепочке вычислений. Это свойство будет удалено через 12 месяцев, начиная с мая 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные с формулами, чтобы создать зависимости
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Получить ячейку, у которой есть зависимые
                Cell cell = worksheet.Cells["A1"];

                // Вызовите GetLeafs с параметром recursive, установленным в true
                IEnumerator leafs = cell.GetLeafs(true);

                // Отобразите результаты
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Сохраните книгу
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


