---
title: RunAllFormulas
second_title: Aspose.Cells for .NET API Referansı
description: Tüm hücrelerin formülünü çalıştırır.
type: docs
weight: 770
url: /tr/net/aspose.cells.griddesktop/griddesktop/runallformulas/
---
## GridDesktop.RunAllFormulas method

Tüm hücrelerin formülünü çalıştırır.

```csharp
public void RunAllFormulas()
```

### Örnekler

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->