---
title: Replace
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Sostituisce il valore di una cella con una nuova stringa.
type: docs
weight: 570
url: /it/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Sostituisce il valore di una cella con una nuova stringa.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValue | String | Valore stringa da sostituire |

### Esempi

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

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Sostituisce il valore di una cella con un nuovo intero.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValue | Int32 | Valore intero da sostituire |

### Esempi

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

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Sostituisce il valore di una cella con un nuovo double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValue | Double | Doppio valore da sostituire |

### Esempi

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

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Sostituisce il valore di una cella con un nuovo array di stringhe.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValues | String[] | Matrice di stringhe da sostituire |
| isVertical | Boolean | Vero - Verticale, Falso - Orizzontale |

### Esempi

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

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Sostituisce i valori delle celle con un array intero.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValues | Int32[] | Matrice intera da sostituire |
| isVertical | Boolean | Vero - Verticale, Falso - Orizzontale |

### Esempi

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

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Sostituisce i valori delle celle con un doppio array.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValues | Double[] | Doppio array da sostituire |
| isVertical | Boolean | Vero - Verticale, Falso - Orizzontale |

### Esempi

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

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Sostituisce i valori delle celle con i dati di aDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| insertTable | DataTable | DataTable da sostituire |

### Esempi

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Aggiunge dati a myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Aggiunge dati a myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Sostituisce i valori delle celle con nuovi dati.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| boolValue | Boolean | Il valore booleano da sostituire. |
| newValue | Object | Nuovo valore. Può essere un valore stringa, intero, doppio o DateTime. |

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Sostituisce i valori delle celle con nuovi dati.

```csharp
public int Replace(int intValue, object newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intValue | Int32 | Il valore intero da sostituire. |
| newValue | Object | Nuovo valore. Può essere un valore stringa, intero, doppio o DateTime. |

### Guarda anche

* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Sostituisce il valore di una cella con una nuova stringa.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| placeHolder | String | Segnaposto di cella |
| newValue | String | Valore stringa da sostituire |
| options | ReplaceOptions | Le opzioni di sostituzione |

### Guarda anche

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
