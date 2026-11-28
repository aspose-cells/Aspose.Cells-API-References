---
title: "Enum ControlMousePointerType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType enum. Kontrol için fare imlecinde gösterilen simge tipini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Denetim için fare imlecinde görüntülenen simge türünü temsil eder.

```csharp
public enum ControlMousePointerType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Standart işaretçi. |
| Arrow | `1` | Ok. |
| Cross | `2` | Nişangah işaretçisi. |
| IBeam | `3` | I-çubuğu. |
| SizeNESW | `6` | Kuzeydoğu ve güneybatı yönlerine işaret eden çift ok. |
| SizeNS | `7` | Kuzey ve güney yönlerine işaret eden çift ok. |
| SizeNWSE | `8` | Kuzeybatı ve güneydoğu yönlerine işaret eden çift ok. |
| SizeWE | `9` | Batı ve doğu yönlerine işaret eden çift ok. |
| UpArrow | `10` | Yukarı ok. |
| HourGlass | `11` | Kum saati. |
| NoDrop | `12` | "Not" sembolü (çapraz çizgili daire), sürüklenen nesnenin üstünde. |
| AppStarting | `13` | Kum saatiyle ok. |
| Help | `14` | Soru işaretiyle ok. |
| SizeAll | `15` | "Size-all" imleci (kuzeye, güneye, doğuya ve batıya işaret eden oklar). |
| Custom | `99` | MouseIcon özelliğiyle belirtilen simgeyi kullanır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // ActiveXControl'ü ActiveXControlBase'e dönüştürerek özelliklerine erişin
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Kontrol için fare işaretçi tipini ayarlayın
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Demonstrasyon için diğer özellikleri ayarlayın
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Sonucu çıktı olarak ver
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


