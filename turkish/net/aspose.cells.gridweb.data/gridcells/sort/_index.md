---
title: "GridCells.Sort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCells yöntemi. Belirtilen sütun indeksine göre bir Çalışma Sayfası aralığında verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksine göre bir Çalışma Sayfası aralığında verileri soldan sağa artan/azalan şekilde sıralar."
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Ayrıca Bakınız

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Belirtilen sütun indeksine göre bir Çalışma Sayfası aralığındaki verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksine göre bir Çalışma Sayfası aralığındaki verileri soldan sağa artan/azalan şekilde sıralar.

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
| indeksler | Int32[] | Sıralama sütununu belirten sütun indeks dizisi. Orientation üstten alta ise, sıralama sütununu belirten sütun indeksini temsil eder. Orientation soldan sağa ise, sıralama satırını belirten satır indeksini temsil eder. |
| sıralamalar | SortByOrder[] | sıralama düzeni dizisi. |
| yönlendirme | SortOrientation | sıralama yönü |
| isCaseSensitive | Boolean | sıralamanın büyük/küçük harfe duyarlı olup olmadığı . |

### Örnekler

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### Ayrıca Bakınız

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


