---
title: Replace
second_title: Aspose.Cells für .NET-API-Referenz
description: Ersetzt den Wert einer Zelle durch eine neue Zeichenfolge.
type: docs
weight: 570
url: /de/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Ersetzt den Wert einer Zelle durch eine neue Zeichenfolge.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValue | String | Zu ersetzender Zeichenfolgenwert |

### Beispiele

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

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Ersetzt den Wert einer Zelle durch eine neue Ganzzahl.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValue | Int32 | Zu ersetzender ganzzahliger Wert |

### Beispiele

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

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Ersetzt den Wert einer Zelle durch ein neues Double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValue | Double | Doppelter Wert zum Ersetzen |

### Beispiele

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

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Ersetzt den Wert einer Zelle durch ein neues String-Array.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValues | String[] | Zu ersetzendes String-Array |
| isVertical | Boolean | True – Vertikal, False – Horizontal |

### Beispiele

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

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Ersetzt die Werte der Zellen durch ein Integer-Array.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValues | Int32[] | Zu ersetzendes Integer-Array |
| isVertical | Boolean | True – Vertikal, False – Horizontal |

### Beispiele

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

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Ersetzt die Werte der Zellen durch ein doppeltes Array.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValues | Double[] | Double-Array zu ersetzen |
| isVertical | Boolean | True – Vertikal, False – Horizontal |

### Beispiele

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

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Ersetzt die Werte der Zellen durch Daten aus aDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| insertTable | DataTable | DataTable zu ersetzen |

### Beispiele

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Fügt Daten zu myDataTable hinzu
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Fügt Daten zu myDataTable hinzu
............
workbook.Replace("AnOldValue", myDataTable)
```

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Ersetzt die Werte der Zellen durch neue Daten.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| boolValue | Boolean | Der zu ersetzende boolesche Wert. |
| newValue | Object | Neuer Wert. Kann ein String-, Integer-, Double- oder DateTime-Wert sein. |

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Ersetzt die Werte der Zellen durch neue Daten.

```csharp
public int Replace(int intValue, object newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intValue | Int32 | Der zu ersetzende ganzzahlige Wert. |
| newValue | Object | Neuer Wert. Kann ein String-, Integer-, Double- oder DateTime-Wert sein. |

### Siehe auch

* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Ersetzt den Wert einer Zelle durch eine neue Zeichenfolge.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | String | Zellplatzhalter |
| newValue | String | Zu ersetzender Zeichenfolgenwert |
| options | ReplaceOptions | Die Ersetzungsoptionen |

### Siehe auch

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* namensraum [Aspose.Cells](../../workbook)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
