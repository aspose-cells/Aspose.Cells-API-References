---
title: "OleObject.AutoUpdate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. OleObject'e olan bağlantının otomatik olarak güncellenip güncellenmeyeceğini belirtir."
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

OleObject bağlantısının otomatik olarak güncellenip güncellenmeyeceğini belirtir.

```csharp
public bool AutoUpdate { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Demonstrasyon için örnek dosyalar oluştur
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Mevcut değilse örnek görüntü dosyası oluştur
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Mevcut değilse örnek Excel dosyası oluştur
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Görüntü verisini oku
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Çalışma sayfasına OleObject ekle
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // OleObject özelliklerini ayarla
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // AutoUpdate özelliğini göster
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


