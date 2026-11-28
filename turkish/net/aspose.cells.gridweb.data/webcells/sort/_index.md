---
title: "WebCells.Sort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebCells yöntemi. Belirtilen sütun indeksine göre bir WebWorksheet aralığındaki verileri yukarıdan aşağıya sıralar."
type: docs
url: /tr/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

WebWorksheet aralığında belirtilen sütun indeksine göre verileri yukarıdan aşağıya artan şekilde sıralar.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| indeks | Int32 | Sıralama sütununu belirten sütun indeksi. |

### Örnekler

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### Ayrıca Bakınız

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

WebWorksheet aralığında belirtilen sütun indeksine göre verileri yukarıdan aşağıya artan şekilde sıralar.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| indeks | Int32 | Sıralama sütununu (veya satırını) belirten sütun (veya satır) indeksi. Sıralama yönü yukarıdan aşağıya ise indeks sütun indeksini, soldan sağa ise indeks satır indeksini temsil eder. |
| sıralama | SortByOrder | Sıralama düzeni: Artan veya Azalan |
| yönlendirme | SortOrientation | Sıralama yönü: yukarıdan aşağıya veya soldan sağa. |
| isCaseSensitive | Boolean | Veri bir dize ise sıralama verisinin büyük/küçük harfe duyarlı olup olmadığını gösterir. |

### Örnekler

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### Ayrıca Bakınız

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

WebWorksheet aralığında, sütun indeksleri dizisiyle belirtilen bazı alanlara göre verileri yukarıdan aşağıya artan şekilde sıralar.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| indeksler | Int32[] | Verinin sıralandığı sütun indekslerini belirten sütun indeksleri dizisi. |

### Örnekler

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### Ayrıca Bakınız

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

WebWorksheet aralığında, indeks dizisiyle belirtilen bazı alanlara göre verileri artan şekilde sıralar.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| indeksler | Int32[] | Sıralama sütununu (veya satırını) belirten sütun (veya satır) indeksi. Sıralama yönü yukarıdan aşağıya ise indeks sütun indeksini, soldan sağa ise indeks satır indeksini temsil eder. |
| sıralamalar | SortByOrder[] | Sıralama düzeni: Artan veya Azalan |
| yönlendirme | SortOrientation | Sıralama yönü: yukarıdan aşağıya veya soldan sağa. |
| isCaseSensitive | Boolean | Sıralamanın büyük/küçük harfe duyarlı olup olmadığını gösterir. |

### Açıklamalar

Bu yöntemi bir veri bloğunu sıralamak için kullanıyorsanız, indeks parametresinin uzunluğunun sipariş parametresinin uzunluğuna eşit olduğundan emin olun.

### Örnekler

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### Ayrıca Bakınız

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


