---
title: Replace
second_title: Aspose.Cells for .NET API Referansı
description: Bir hücrenin değerini yeni bir dizeyle değiştirir.
type: docs
weight: 570
url: /tr/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Bir hücrenin değerini yeni bir dizeyle değiştirir.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValue | String | Değiştirilecek dize değeri |

### Örnekler

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

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Bir hücrenin değerini yeni bir tamsayı ile değiştirir.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValue | Int32 | Değiştirilecek tamsayı değeri |

### Örnekler

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

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Bir hücrenin değerini yeni bir double ile değiştirir.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValue | Double | Değiştirilecek çift değer |

### Örnekler

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

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Bir hücrenin değerini yeni bir dize dizisiyle değiştirir.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValues | String[] | Değiştirilecek dize dizisi |
| isVertical | Boolean | Doğru - Dikey, Yanlış - Yatay |

### Örnekler

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

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Hücrelerin değerlerini bir tamsayı dizisiyle değiştirir.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValues | Int32[] | Değiştirilecek tamsayı dizisi |
| isVertical | Boolean | Doğru - Dikey, Yanlış - Yatay |

### Örnekler

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

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Hücrelerin değerlerini bir çift diziyle değiştirir.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValues | Double[] | Değiştirilecek çift dizi |
| isVertical | Boolean | Doğru - Dikey, Yanlış - Yatay |

### Örnekler

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

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Hücrelerin değerlerini birDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| insertTable | DataTable | Değiştirilecek DataTable |

### Örnekler

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// myDataTable'a veri ekler
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' myDataTable'a veri ekler
............
workbook.Replace("AnOldValue", myDataTable)
```

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Hücrelerin değerlerini yeni verilerle değiştirir.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| boolValue | Boolean | Değiştirilecek boole değeri. |
| newValue | Object | Yeni değer. Dize, tamsayı, çift veya DateTime değeri olabilir. |

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Hücrelerin değerlerini yeni verilerle değiştirir.

```csharp
public int Replace(int intValue, object newValue)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| intValue | Int32 | Değiştirilecek tamsayı değeri. |
| newValue | Object | Yeni değer. Dize, tamsayı, çift veya DateTime değeri olabilir. |

### Ayrıca bakınız

* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Bir hücrenin değerini yeni bir dizeyle değiştirir.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| placeHolder | String | Hücre yer tutucusu |
| newValue | String | Değiştirilecek dize değeri |
| options | ReplaceOptions | Değiştirme seçenekleri |

### Ayrıca bakınız

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* ad alanı [Aspose.Cells](../../workbook)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
