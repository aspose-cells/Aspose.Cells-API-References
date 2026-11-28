---
title: "Enum ControlPicturePositionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Denetimin resminin başlığına göre konumunu temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Denetimin resminin, başlığa göre konumunu temsil eder.

```csharp
public enum ControlPicturePositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LeftTop | `131072` | Resim, başlığın solunda görünür. Başlık, resmin üst kısmına hizalanmıştır. |
| LeftCenter | `327683` | Resim, başlığın solunda görünür. Başlık, resme göre ortalanmıştır. |
| LeftBottom | `524294` | Resim, başlığın solunda görünür. Başlık, resmin alt kısmına hizalanmıştır. |
| RightTop | `2` | Resim, başlığın sağında görünür. Başlık, resmin üst kısmına hizalanmıştır. |
| RightCenter | `196613` | Resim, başlığın sağında görünür. Başlık, resme göre ortalanmıştır. |
| RightBottom | `393224` | Resim, başlığın sağında görünür. Başlık, resmin alt kısmına hizalanmıştır. |
| AboveLeft | `393216` | Resim, başlığın üstünde görünür. Başlık, resmin sol kenarına hizalanmıştır. |
| AboveCenter | `458753` | Resim, başlığın üstünde görünür. Başlık, resmin altında ortalanmıştır. |
| AboveRight | `524290` | Resim, başlığın üstünde görünür. Başlık, resmin sağ kenarına hizalanmıştır. |
| BelowLeft | `6` | Resim, başlığın altında görünür. Başlık, resmin sol kenarına hizalanmıştır. |
| BelowCenter | `65543` | Resim, başlığın altında görünür. Başlık, resmin üzerinde ortalanmıştır. |
| BelowRight | `131080` | Resim, başlığın altında görünür. Başlık, resmin sağ kenarına hizalanmıştır. |
| Center | `262148` | Resim, kontrolün ortasında görünür. Başlık, resmin üzerinde yatay ve dikey olarak ortalanmıştır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPicturePositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 0, 1, 0, 100, 50);
            ToggleButtonActiveXControl activeXControl = (ToggleButtonActiveXControl)shape.ActiveXControl;

            activeXControl.Caption = "Demo Button";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.IsAutoSize = true;

            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


