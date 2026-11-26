---
title: "Cell.PutValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Помещает логическое значение в ячейку"
type: docs
url: /ru/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Записывает логическое значение в ячейку.

```csharp
public void PutValue(bool boolValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| boolValue | Boolean |  |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Поместить логическое значение в ячейку B3 (строка 2, столбец 2)
            cells[2, 2].PutValue(true);

            // Проверить, что значение было установлено правильно
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Записывает целочисленное значение в ячейку.

```csharp
public void PutValue(int intValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| intValue | Int32 | Входное значение |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Использование PutValue с параметрами типа Int32
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Вычислить сумму значений
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Записывает значение double в ячейку.

```csharp
public void PutValue(double doubleValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleValue | Double | Входное значение |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Поместить значения типа double с помощью метода PutValue
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Сохраните книгу
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Записывает значение в ячейку; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | String | Входное значение |
| isConverted | Boolean | True: преобразовано в другой тип данных, если это уместно. |
| setStyle | Boolean | True: установить числовой формат в стиль ячейки при преобразовании в другой тип данных |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить ячейку B3
            Cell cell = worksheet.Cells["B3"];
            
            // Установить проверку данных для возраста (должно быть положительное число)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Поместить значение с преобразованием и проверкой валидности
            cell.PutValue("-60", true, false);
            
            // Вычислить формулы (хотя в этом простом случае это не требуется)
            workbook.CalculateFormula();
            
            // Проверить, является ли значение допустимым
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Сохранить книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Записывает строковое значение в ячейку и при необходимости преобразует его в другой тип данных.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | String | Входное значение |
| isConverted | Boolean | True: преобразовано в другой тип данных, если это уместно. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Продемонстрировать PutValue со строковыми и логическими параметрами
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Проверьте значения
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Записывает строковое значение в ячейку.

```csharp
public void PutValue(string stringValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stringValue | String | Входное значение |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Использование PutValue со строковыми параметрами
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Сохраните книгу
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Записывает значение DateTime в ячейку.

```csharp
public void PutValue(DateTime dateTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dateTime | DateTime | Входное значение |

### Примечания

Установка значения DateTime для ячейки не означает, что ячейка будет автоматически отформатирована как дата и время. Значение DateTime хранится как числовое значение в модели данных как MS Excel, так и Aspose.Cells. Будет ли числовое значение интерпретировано как само число или как дата и время, зависит от числового формата, применённого к этой ячейке. Если эта ячейка не отформатирована как дата и время, она будет отображаться как числовое значение, даже если вы ввели DateTime.

### Примеры

Этот пример показывает, как установить значение DateTime в ячейку и заставить его отображаться как дата и время.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Поместите дату и время в ячейку
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Записывает объектное значение в ячейку.

```csharp
public void PutValue(object objectValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| objectValue | Object | входное значение |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue с объектом DateTime
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue с объектом string
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue с объектом numeric
            cells[2, 0].PutValue((object)123.45);
            
            // Сохраните книгу
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


