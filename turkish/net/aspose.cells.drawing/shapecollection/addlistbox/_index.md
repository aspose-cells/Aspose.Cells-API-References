---
title: AddListBox
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma sayfasına bir Liste Kutusu ekler.
type: docs
weight: 170
url: /tr/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Çalışma sayfasına bir Liste Kutusu ekler.

```csharp
public ListBox AddListBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| top | Int32 | Piksel biriminde, ListBox'ın sol satırından dikey uzaklığını temsil eder. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| left | Int32 | ListBox'ın sol sütunundan piksel birimi cinsinden yatay uzaklığını temsil eder. |
| height | Int32 | Piksel biriminde ListBox'ın yüksekliğini temsil eder. |
| width | Int32 | Piksel biriminde ListBox genişliğini temsil eder. |

### Geri dönüş değeri

Bir ListBox nesnesi.

### Örnekler

```csharp

[C#]
//liste kutusu ekle
ListBox listBox = shapes.AddListBox(1, 0, 1, 0, 100, 50);
```

### Ayrıca bakınız

* class [ListBox](../../listbox)
* class [ShapeCollection](../../shapecollection)
* ad alanı [Aspose.Cells.Drawing](../../shapecollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
