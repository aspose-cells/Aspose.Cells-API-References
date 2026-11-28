---
title: "Sınıf UnknownControl"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.UnknownControl sınıfı. Bilinmeyen kontrol"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

Bilinmeyen denetim.

```csharp
public class UnknownControl : ActiveXControl
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Arka planın ole rengini alır ve ayarlar. ([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | Kontrolün ikili verilerini alır ve ayarlar. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Kontrolün yazı tipini temsil eder. ([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Ön planın ole rengini alır ve ayarlar. ([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Kontrolün yüksekliğini puan biriminde alır ve ayarlar. ([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Kontrol odaklandığında Input Method Editor'ün varsayılan çalışma zaman modunu alır ve ayarlar. ([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Kontrolün tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. ([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Kontrolün odak alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. ([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Kontrol içindeki verinin düzenleme için kilitli olup olmadığını gösterir. ([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Denetimin şeffaf olup olmadığını gösterir.([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Denetimin görünür olup olmadığını gösterir.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Bağlı hücreyi alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Liste doldurma aralığını alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Denetim için fare imleci olarak gösterilecek özel bir simgeyi alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Denetim için fare imleci olarak gösterilen simge türünü alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Gölge gösterilip gösterilmeyeceğini belirtir.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder.([`ActiveXControl`](../activexcontrol/) üzerinden devralınmıştır.) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | ActiveX denetiminin türünü alır. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Denetimin genişliğini puan biriminde alır ve ayarlar.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | [`Workbook`](../activexcontrolbase/workbook/) nesnesini alır.([`ActiveXControlBase`](../activexcontrolbase/) üzerinden devralınmıştır.) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | İlgili verileri alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassUnknownControlDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir Unknown ActiveX kontrolü ekleyin
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // Şekilden UnknownControl örneğini alın
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // Çalışma kitabını kaydedin
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


