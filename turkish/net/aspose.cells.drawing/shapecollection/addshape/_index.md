---
title: AddShape
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma sayfasına bir Şekil ekler.
type: docs
weight: 260
url: /tr/net/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection.AddShape method

Çalışma sayfasına bir Şekil ekler.

```csharp
public Shape AddShape(MsoDrawingType type, int upperLeftRow, int top, int upperLeftColumn, 
    int left, int height, int width)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| type | MsoDrawingType | Mso çizim türü. |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| top | Int32 | Şekil öğesinin sol satırından piksel birimi cinsinden dikey uzaklığını temsil eder. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| left | Int32 | Şekil öğesinin sol sütunundan piksel birimi cinsinden yatay uzaklığını temsil eder. |
| height | Int32 | Şeklin yüksekliğini piksel biriminde temsil eder. |
| width | Int32 | Piksel biriminde Şekil genişliğini temsil eder. |

### Geri dönüş değeri

Bir Shape nesnesi.

### Notlar

Tür, Chart/Comment/Picture/OleObject/Polygon/DialogBox olamaz

### Örnekler

```csharp

[C#]
//Belirtilen türden bir şekil ekleyin
Shape shapeByType = shapes.AddShape(MsoDrawingType.CellsDrawing, 1, 0, 1, 0, 100, 50);
```

### Ayrıca bakınız

* class [Shape](../../shape)
* enum [MsoDrawingType](../../msodrawingtype)
* class [ShapeCollection](../../shapecollection)
* ad alanı [Aspose.Cells.Drawing](../../shapecollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
