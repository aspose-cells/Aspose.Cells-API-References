---
title: "Sınıf ActiveXControl"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControl sınıfı. ActiveX kontrolünü temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

ActiveX denetimini temsil eder.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Arka planın ole rengini alır ve ayarlar. ([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Kontrolün ikili verilerini alır ve ayarlar. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Kontrolün yazı tipini temsil eder. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Ön planın ole rengini alır ve ayarlar. ([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Kontrolün yüksekliğini puan biriminde alır ve ayarlar. ([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Kontrol odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modu alır ve ayarlar. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Kontrolün tüm içeriğini göstermek için otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını belirtir. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Kontrolün odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini belirtir. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Kontrol içindeki verilerin düzenleme için kilitli olup olmadığını belirtir. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Kontrolün şeffaf olup olmadığını belirtir. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Denetimin görünür olup olmadığını gösterir.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Bağlı hücreyi alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Liste doldurma aralığını alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Denetim için fare imleci olarak gösterilen simge türünü alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Gölge gösterilip gösterilmeyeceğini belirtir.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Kontrolün metni nasıl hizalanacağını temsil eder. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | ActiveX kontrolünün tipini alır.(`[`ActiveXControlBase`](../activexcontrolbase/)` üzerinden devralınmıştır.) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Denetimin genişliğini puan biriminde alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | [`Workbook`](../activexcontrolbase/workbook/) nesnesini alır.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassActiveXControlDemo
    {
        public static void Run()
        {
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // RadioButton ActiveX kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Özellikleri ayarla
            radioButton.GroupName = "Sheet1";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;
            radioButton.Caption = "OptionButton1";
            radioButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            radioButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            radioButton.IsEnabled = true;
            radioButton.IsTransparent = false;
            radioButton.IsAutoSize = false;
            radioButton.IMEMode = InputMethodEditorMode.NoControl;
            radioButton.Font.Name = "Calibri";
            radioButton.MousePointer = ControlMousePointerType.Default;

            // Çalışma kitabını kaydedin
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


