---
title: "Enum ControlMatchEntryType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType enum. Kullanıcı yazarken bir ListBox veya ComboBox'ın listesini nasıl aradığını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

Bir ListBox veya ComboBox'un, kullanıcının yazarken listesini nasıl aradığını temsil eder.

```csharp
public enum ControlMatchEntryType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| FirstLetter | `0` | Kontrol, girilen karakterle başlayan bir sonraki girişi arar. Aynı harfi tekrar tekrar yazmak, o harfle başlayan tüm girdiler arasında döner. |
| Complete | `1` | Her karakter girildiğinde, kontrol girilen tüm karakterlere uyan bir girişi arar. |
| None | `2` | Karakterler girildiğinde liste aranmayacaktır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ControlMatchEntryTypeDemo
    {
        public static void ControlMatchEntryTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Çalışma sayfasına bir ComboBox ActiveX denetimi ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // ComboBox için özellikleri ayarla
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // ComboBox'a öğeler ekle
            comboBox.Value = "Apple;Banana;Cherry";

            // Çalışma sayfasına bir ListBox ActiveX denetimi ekle
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // ListBox için özellikleri ayarla
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // ListBox'a öğeler ekle
            listBox.Value = "Apple;Banana;Cherry";

            // Çalışma kitabını kaydedin
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


