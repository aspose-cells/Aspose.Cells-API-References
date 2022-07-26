---
title: Replace
second_title: Référence de l'API Aspose.Cells pour .NET
description: Remplace la valeur dune cellule par une nouvelle chaîne.
type: docs
weight: 570
url: /fr/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Remplace la valeur d'une cellule par une nouvelle chaîne.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | String | Valeur de chaîne à remplacer |

### Exemples

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

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Remplace la valeur d'une cellule par un nouvel entier.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | Int32 | Valeur entière à remplacer |

### Exemples

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

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Remplace la valeur d'une cellule par un nouveau double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | Double | Double valeur à remplacer |

### Exemples

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

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Remplace la valeur d'une cellule par un nouveau tableau de chaînes.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValues | String[] | Tableau de chaînes à remplacer |
| isVertical | Boolean | Vrai - Vertical, Faux - Horizontal |

### Exemples

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

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Remplace les valeurs des cellules par un tableau d'entiers.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValues | Int32[] | Tableau d'entiers à remplacer |
| isVertical | Boolean | Vrai - Vertical, Faux - Horizontal |

### Exemples

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

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Remplace les valeurs des cellules par un double tableau.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValues | Double[] | Double tableau à remplacer |
| isVertical | Boolean | Vrai - Vertical, Faux - Horizontal |

### Exemples

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

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Remplace les valeurs des cellules par les données d'unDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| insertTable | DataTable | DataTable à remplacer |

### Exemples

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Ajoute des données à myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Ajoute des données à myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Remplace les valeurs des cellules par de nouvelles données.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| boolValue | Boolean | Valeur booléenne à remplacer. |
| newValue | Object | Nouvelle valeur. Peut être une chaîne, un entier, un double ou une valeur DateTime. |

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Remplace les valeurs des cellules par de nouvelles données.

```csharp
public int Replace(int intValue, object newValue)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| intValue | Int32 | La valeur entière à remplacer. |
| newValue | Object | Nouvelle valeur. Peut être une chaîne, un entier, un double ou une valeur DateTime. |

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Remplace la valeur d'une cellule par une nouvelle chaîne.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | String | Valeur de chaîne à remplacer |
| options | ReplaceOptions | Les options de remplacement |

### Voir également

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
