---
title: "Cells.ImportObjectArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Импортирует массив данных в лист"
type: docs
url: /ru/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

Импортирует массив данных в лист.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | Object[] | Массив данных. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| isVertical | Boolean | Указывает импортировать данные вертикально или горизонтально. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте массив объектов с примерными данными
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // Импортируйте массив объектов в лист, начиная с ячейки B3 (строка 2, столбец 1), горизонтально
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Сохраните книгу, чтобы продемонстрировать результат
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

Импортирует массив данных в лист.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| objArray | Object[] | Массив данных. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| isVertical | Boolean | Указывает импортировать данные вертикально или горизонтально. |
| пропустить | Int32 | Количество пропущенных строк или столбцов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Подготовьте данные для параметров ImportObjectArray: (Object[], Int32, Int32, Boolean, Int32)
            object[] data = new object[]
            {
                "Name",
                "Age",
                "Date",
                "John Doe",
                30,
                new DateTime(2023, 10, 15),
                "Jane Smith",
                28,
                new DateTime(2023, 10, 16)
            };

            try
            {
                // Вызовите ImportObjectArray с параметрами: (массив данных, начальная строка 0, начальный столбец 0, горизонтальный импорт, пропустить 1 столбец между записями)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // Продемонстрировать эффект: данные будут размещены в ячейках A1, C1, E1, A2, C2, E2 и т.д., при пропуске столбцов
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


