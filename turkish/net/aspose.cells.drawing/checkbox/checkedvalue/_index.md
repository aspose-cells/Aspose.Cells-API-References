---
title: "CheckBox.CheckedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBox özelliği. Onay kutusu değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Onay kutusunun değerini alır veya ayarlar.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir onay kutusu ekle
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Onay kutusu değerini İşaretli olarak ayarla
            checkBox.CheckedValue = CheckValueType.Checked;

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Kaydedilmiş çalışma kitabını doğrulamak için yükle
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Onay kutusu durumunu çıktı olarak ver
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### Ayrıca Bakınız

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


