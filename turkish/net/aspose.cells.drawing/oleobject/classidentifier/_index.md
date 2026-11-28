---
title: "OleObject.ClassIdentifier"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Gömülü nesnenin sınıf tanımlayıcısını alır ve ayarlar. Bu, gömülü dosyayı hangi uygulamanın açacağını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Gömülü nesnenin sınıf tanımlayıcısını alır ve ayarlar. Bu, gömülü dosyayı hangi uygulamanın açtığını gösterir.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ClassIdentifier için örnek bayt dizisi (normalde bu gerçek bir sınıf kimliği olurdu)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // Örnek veriyle bir OLE nesnesi ekle
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // ClassIdentifier özelliğini ayarla
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectDemo.xlsx");

            // Kaydedilmiş çalışma kitabını yükle ve ClassIdentifier'ı doğrula
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // ClassIdentifier'ın korunduğunu doğrulayın
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


