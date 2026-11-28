---
title: "GridCell.Formula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridCell özelliği. GridCell'in formülünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

[`GridCell`](../) formülünü alır veya ayarlar.

```csharp
public string Formula { get; set; }
```

### Açıklamalar

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül (,) kullanın, örneğin "=SUM(A1, E1, H2)".

Kullanıcı, Workbook tasarım dosyasında herhangi bir formül ayarlayabilir. Aspose.Cells tüm formülleri korur. Kullanıcı bu özelliği bir hücreye formül ayarlamak için kullanırsa, Workbook yerleşik işlevlerinin büyük bir kısmı desteklenir. Ve daha fazlası geliyor. Workbook yerleşik işlevleri için özel bir ihtiyacınız varsa, lütfen bize bildirin.

### Örnekler

```csharp
[C#]

ridWeb GridWeb1 = new GridWeb();
ridWorksheet sheet = GridWeb1.ActiveSheet;
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

Visual Basic]

im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### Ayrıca Bakınız

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


