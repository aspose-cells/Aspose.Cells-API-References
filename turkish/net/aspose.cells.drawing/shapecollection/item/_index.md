---
title: Item
second_title: Aspose.Cells for .NET API Referansı
description: Belirli bir dizindeki şekil nesnesini alır.
type: docs
weight: 10
url: /tr/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Belirli bir dizindeki şekil nesnesini alır.

```csharp
public Shape this[int index] { get; }
```

| Parametre | Tanım |
| --- | --- |
| index |  |

### Örnekler

```csharp

[C#]
//şekli al
Shape shape = shapes[shapes.Count -1];
```

### Ayrıca bakınız

* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* ad alanı [Aspose.Cells.Drawing](../../shapecollection)
* toplantı [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Şekil nesnesini şekle göre alır image

```csharp
public Shape this[string name] { get; }
```

| Parametre | Tanım |
| --- | --- |
| name |  |

### Örnekler

```csharp

[C#]
//şekil ekle
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//şekli al
Shape shape1 = shapes["Rectangle 1"];
if(shape1 != null)
{
    //'Dikdörtgen 1' adlı şekli aldık.
}
```

### Ayrıca bakınız

* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* ad alanı [Aspose.Cells.Drawing](../../shapecollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
