---
title: "GridCells.Sort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCells yöntemi. Belirtilen sütun indeksine göre bir Çalışma Sayfası aralığında verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksine göre bir Çalışma Sayfası aralığında verileri soldan sağa artan/azalan şekilde sıralar."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Belirtilen sütun indeksine göre bir Çalışma Sayfası aralığındaki verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksine göre bir Çalışma Sayfası aralığındaki verileri soldan sağa artan/azalan şekilde sıralar.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Sıralanacak ilk hücrenin satır numarası. |
| startColumn | Int32 | Sıralanacak ilk hücrenin sütun numarası. |
| satırlar | Int32 | İçe aktarılacak satır sayısı. |
| sütunlar | Int32 | İçe aktarılacak sütun sayısı. |
| indeks | Int32 | Sıralama sütununu belirten sütun indeksi. Yönlendirme yukarıdan aşağıya ise, sıralama sütununu belirten sütun indeksini temsil eder. Yönlendirme soldan sağa ise, sıralama satırını belirten satır indeksini temsil eder. |
| isAsending | Boolean | sıralama düzeninin artan olup olmadığı . |
| isCaseSensitive | Boolean | sıralamanın büyük/küçük harfe duyarlı olup olmadığı . |
| islefttoright | Boolean | sıralama yönünün soldan sağa olup olmadığı |

### Örnekler

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Ayrıca Bakınız

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Alan verilerini sıralar.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parametre | Açıklama |
| --- | --- |
| hücreler | Hücreler veri alanını içerir. |
| startRow | Alanının başlangıç satırı. |
| startColumn | Alanının başlangıç sütunu. |
| satırlar | toplam satır sayısı. |
| sütunlar | Toplam sütun sayısı. |
| indeksler | Sıralanmış sütun indeks dizisi |
| sıralamalar | Sıralanmış sıralama dizisi |
| yönlendirme | sıralama yönü: soldan sağa veya yukarıdan aşağıya. |
| isCaseSensitive | karşılaştırma sırasında büyük/küçük harfe duyarlı olup olmadığı.. |

### Ayrıca Bakınız

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


