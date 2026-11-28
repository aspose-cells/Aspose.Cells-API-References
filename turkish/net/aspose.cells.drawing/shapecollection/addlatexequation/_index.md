---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. LaTeX biçimindeki dizgileri kullanarak çalışma sayfasına bir denklem nesnesi ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Çalışma sayfasına LaTeX biçim dizesi kullanarak bir denklem nesnesi ekler.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Üst satır indeksi. |
| üst | Int32 | Üst satırının dikey kayması, piksel biriminde. |
| leftColumn | Int32 | Sol sütun indeksi. |
| sol | Int32 | Sol sütunundan yatay kaydırma, piksel biriminde. |
| yükseklik | Int32 | Denklemin yüksekliği, piksel biriminde. |
| genişlik | Int32 | Denklemin genişliği, piksel biriminde. |
| latex | String | LaTeX format dizesi |

### Örnekler

```csharp

[C#]
// LaTeX format dizesi.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Çalışma sayfasına bir denklem nesnesi ekler.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### Ayrıca Bakınız

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


