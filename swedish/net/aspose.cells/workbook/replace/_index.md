---
title: Replace
second_title: Aspose.Cells för .NET API-referens
description: Ersätter en cells värde med en ny sträng.
type: docs
weight: 570
url: /sv/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Ersätter en cells värde med en ny sträng.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValue | String | Strängvärde att ersätta |

### Exempel

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

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Ersätter en cells värde med ett nytt heltal.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValue | Int32 | Heltalsvärde som ska ersättas |

### Exempel

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

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Ersätter en cells värde med en ny dubbel.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValue | Double | Dubbelt värde att byta ut |

### Exempel

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

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Ersätter en cells värde med en ny strängmatris.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValues | String[] | Strängarray att ersätta |
| isVertical | Boolean | Sant - Vertikalt, Falskt - Horisontellt |

### Exempel

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

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Ersätter cellvärden med en heltalsmatris.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValues | Int32[] | Heltalsmatris att ersätta |
| isVertical | Boolean | Sant - Vertikalt, Falskt - Horisontellt |

### Exempel

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

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Ersätter cellernas värden med en dubbel array.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValues | Double[] | Dubbel array att byta ut |
| isVertical | Boolean | Sant - Vertikalt, Falskt - Horisontellt |

### Exempel

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

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Ersätter cellernas värden med data från enDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| insertTable | DataTable | DataTable att ersätta |

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Lägger till data till myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Lägger till data till myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Ersätter cellernas värden med nya data.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| boolValue | Boolean | Det booleska värdet som ska ersättas. |
| newValue | Object | Nytt värde. Kan vara sträng, heltal, dubbel eller DateTime värde. |

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Ersätter cellernas värden med nya data.

```csharp
public int Replace(int intValue, object newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intValue | Int32 | Heltalsvärdet som ska ersättas. |
| newValue | Object | Nytt värde. Kan vara sträng, heltal, dubbel eller DateTime värde. |

### Se även

* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Ersätter en cells värde med en ny sträng.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| placeHolder | String | Cellplatshållare |
| newValue | String | Strängvärde att ersätta |
| options | ReplaceOptions | Ersätt alternativen |

### Se även

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* namnutrymme [Aspose.Cells](../../workbook)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
