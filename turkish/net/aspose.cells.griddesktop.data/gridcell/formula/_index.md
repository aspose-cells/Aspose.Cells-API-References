---
title: "GridCell.Formula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell özelliği. Hücrenin formülünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Hücrenin formülünü alır veya ayarlar.

```csharp
public string Formula { get; set; }
```

### Açıklamalar

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül (,) kullanın, örneğin "=SUM(A1, E1, H2)".

Kullanıcı, Workbook tasarım dosyasında herhangi bir formül ayarlayabilir. Aspose.Cells tüm formülleri korur. Kullanıcı bu özelliği bir hücreye formül ayarlamak için kullanırsa, Workbook yerleşik işlevlerinin büyük bir kısmı desteklenir. Ve daha fazlası geliyor. Workbook yerleşik işlevleri için özel bir ihtiyacınız varsa, lütfen bize bildirin.

### Örnekler

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Ayrıca Bakınız

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


