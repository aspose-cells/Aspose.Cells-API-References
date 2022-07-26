---
title: Replace
second_title: Справочник по Aspose.Cells для .NET API
description: Заменяет значение ячейки новой строкой.
type: docs
weight: 570
url: /ru/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Заменяет значение ячейки новой строкой.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | String | Строковое значение для замены |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
......
workbook.Replace("AnOldValue", "NewValue");

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
 ........
orkbook.Replace("AnOldValue", "NewValue")
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Заменяет значение ячейки новым целым числом.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | Int32 | Целое значение для замены |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
......
int newValue = 100;
workbook.Replace("AnOldValue", newValue);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Integer =  100 
orkbook.Replace("AnOldValue", NewValue)
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Заменяет значение ячейки новым двойным значением.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | Double | Двойное значение для замены |

### Примеры

```csharp

[C#]

Workbook workbook = new Workbook();
......
double newValue = 100.0;
workbook.Replace("AnOldValue", newValue);


[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Double =  100.0
orkbook.Replace("AnOldValue", NewValue)
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Заменяет значение ячейки новым массивом строк.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValues | String[] | Массив строк для замены |
| isVertical | Boolean | Правда — по вертикали, Ложь — по горизонтали |

### Примеры

```csharp

[C#]

Workbook workbook = new Workbook();
......
string[] newValues = new string[]{"Tom", "Alice", "Jerry"};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
.............
im NewValues() As String =  New String() {"Tom", "Alice", "Jerry"}		
orkbook.Replace("AnOldValue", NewValues, True)
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Заменяет значения ячеек массивом целых чисел.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValues | Int32[] | Целочисленный массив для замены |
| isVertical | Boolean | Правда — по вертикали, Ложь — по горизонтали |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
......
int[] newValues = new int[]{1, 2, 3};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
..........
im NewValues() As Integer =  New Integer() {1, 2, 3}
orkbook.Replace("AnOldValue", NewValues, True)
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Заменяет значения ячеек двойным массивом.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValues | Double[] | Двойной массив для замены |
| isVertical | Boolean | Правда — по вертикали, Ложь — по горизонтали |

### Примеры

```csharp

[C#]

Workbook workbook = new Workbook();
......
double[] newValues = new double[]{1.23, 2.56, 3.14159};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
...........
Dim NewValues() As Double =  New Double() {1.23, 2.56, 3.14159}
workbook.Replace("AnOldValue", NewValues, True)
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Заменяет значения ячеек данными изDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| insertTable | DataTable | DataTable для замены |

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Добавляет данные в myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Добавляет данные в myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Заменяет значения ячеек новыми данными.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| boolValue | Boolean | Логическое значение, которое необходимо заменить. |
| newValue | Object | Новое значение. Может быть строкой, целым числом, двойным значением или значением DateTime. |

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Заменяет значения ячеек новыми данными.

```csharp
public int Replace(int intValue, object newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| intValue | Int32 | Заменяемое целочисленное значение. |
| newValue | Object | Новое значение. Может быть строкой, целым числом, двойным значением или значением DateTime. |

### Смотрите также

* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Заменяет значение ячейки новой строкой.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | String | Заполнитель ячейки |
| newValue | String | Строковое значение для замены |
| options | ReplaceOptions | Варианты замены |

### Смотрите также

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* пространство имен [Aspose.Cells](../../workbook)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
