---
title: "OleObject.ObjectSourceFullName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. Bağlantılı OLE nesnesi için kaynak dosyanın tam adını döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Bağlı OLE nesnesi için kaynak dosyanın tam adını döndürür.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Açıklamalar

Yalnızca dosya türü OleFileType.Unknown olduğunda kaynak tam adının ayarlanmasını destekler. Örneğin wav dosyası, avi dosyası vb.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir OLE nesnesi ekle (dosya verisini bayt dizisi olarak kullanarak)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // ObjectSourceFullName'i ayarla ve al
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


