---
title: "CheckBox.Shadow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBox özelliği. Onay kutusunun 3D gölgelendirmeye sahip olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

ComboBox'ın 3D gölgelendirmeye sahip olup olmadığını gösterir.

```csharp
public bool Shadow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir onay kutusu ekle ve indeksini al
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Onay kutusu özelliklerini yapılandır
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Shadow özelliğini göster
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


