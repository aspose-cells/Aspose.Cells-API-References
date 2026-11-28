---
title: "CheckValueType enumı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.CheckValueType enumı. Onay kutusunun kontrol değeri türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Onay kutusunun işaret değeri türünü temsil eder.

```csharp
public enum CheckValueType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| UnChecked | `0` | Seçilmemiş |
| Checked | `1` | Seçilmiş |
| Mixed | `2` | Karışık |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına onay kutuları ekleyin
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Onay kutularını alın ve özelliklerini ayarlayın
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Onay kutusu değerlerini ve işaretli durumunu ayarla
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Onay kutularını hücrelere bağla
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Bağlantıyı göstermek için hücre değerlerini çıktı olarak ver
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


