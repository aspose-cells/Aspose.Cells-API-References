---
title: "PivotField.GroupBy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Автоматически группировать поле с интервалом"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Автоматически группировать поле с интервалом

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| интервал | Double | Внутреннее значение группы. Автоматическое значение будет назначено, если оно равно нулю, |
| newField | Boolean | Указывает, добавляется ли новое поле в сводную таблицу. Только для группировки DateTime. |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Добавить поле в область столбцов
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Группировать поле по 1 (интервал) с автоматическим диапазоном
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Автоматически группировать поле с внутренним

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| группы | PivotGroupByType[] | Типы группировки |
| интервал | Double | Внутреннее значение группы. Автоматическое значение будет назначено, если оно равно нулю, работает только при группировке по числам или дням. |
| newField | Boolean | Указывает, добавляется ли новое поле в сводную таблицу. |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Группировать файл по типам группировки даты.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| начало | DateTime | Начальная дата и время |
| конец | DateTime | Конец даты и времени |
| группы | PivotGroupByType[] | Типы группировки |
| интервал | Double | Интервал |
| firstAsNewField | Boolean | Указывает, добавлять ли новое поле в сводную таблицу. Только для первого элемента группы. |

### Возвращаемое значение

False означает, что это поле нельзя сгруппировать по дате и времени.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные с датами для сводной таблицы
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            // Подготовить параметры для метода GroupBy
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // Вызвать метод GroupBy с параметрами даты
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Обновить сводную таблицу
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Группировать файл по типам группировки даты.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isAutoStart | Boolean | Указывает, следует ли автоматически определять значение начальной даты и времени. |
| начало | DateTime | Начальная дата и время |
| isAutoEnd | Boolean | Указывает, следует ли автоматически определять значение конечной даты и времени. |
| конец | DateTime | Конец даты и времени |
| группы | PivotGroupByType[] | Типы группировки |
| интервал | Double | Интервал |
| firstAsNewField | Boolean | Указывает, добавлять ли новое поле в сводную таблицу. Только для первого элемента группы. |

### Возвращаемое значение

False означает, что это поле нельзя сгруппировать по дате и времени.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Группировать файл по числу.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| начало | Double | Начальное значение |
| конец | Double | Конечное значение |
| интервал | Double | Интервал |
| newField | Boolean | Указывает, добавлять ли новое поле в сводную таблицу |

### Возвращаемое значение

False означает, что это поле нельзя сгруппировать по дате и времени.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки и сгруппировать его
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Сохраните книгу
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Группировать файл по числу.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isAutoStart | Boolean | Указывает, следует ли автоматически определять начальное значение. |
| начало | Double | Начальное значение |
| isAutoEnd | Boolean | Указывает, следует ли автоматически определять конечное значение. |
| конец | Double | Конечное значение |
| интервал | Double | Интервал |
| newField | Boolean | Указывает, добавлять ли новое поле в сводную таблицу |

### Возвращаемое значение

False означает, что это поле нельзя сгруппировать по дате и времени.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions). Этот метод будет удалён через 6 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Пользовательская группировка поля.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | Пользовательские элементы группировки. |
| newField | Boolean | Указывает, добавлять ли новое поле в сводную таблицу |

### Возвращаемое значение

False означает, что это поле нельзя сгруппировать по дате и времени.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions options) с свойством PivotFieldGroupOptions.DiscreteGroupItems. Этот метод будет удалён через 6 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            // Создать пользовательские элементы группы
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Вызвать метод GroupBy с пользовательскими элементами группы
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Обновить сводную таблицу
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Пользовательская группировка поля.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | Пользовательские элементы группировки. |
| newField | Boolean | Указывает, добавлять ли новое поле в сводную таблицу |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.Group(PivotFieldGroupOptions options) с свойством PivotFieldGroupOptions.DiscreteGroupItems. Этот метод будет удалён через 6 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


