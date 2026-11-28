---
title: "ShapeCollection.AddOleObjectWithLinkedImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bağlantılı bir resim ekle"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage/
---
## ShapeCollection.AddOleObjectWithLinkedImage method

Bağlantılı bir resim ekle.

```csharp
public OleObject AddOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| yükseklik | Int32 | Şeklin yüksekliği. Piksel biriminde |
| genişlik | Int32 | Şeklin genişliği. Piksel biriminde |
| sourceFullName | String | Bağlantılı görüntünün kaynak dosyasının yolu ve adı |

### Dönüş Değeri

[`Picture`](../../picture/) Picture object.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddOleObjectWithLinkedImageWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlantı yapılacak görüntü dosyasının yolu
            string imagePath = "example.jpg";

            try
            {
                // Belirli parametrelerle AddOleObjectWithLinkedImage yöntemini çağırın
                OleObject oleObject = worksheet.Shapes.AddOleObjectWithLinkedImage(
                    1,  // upperLeftRow
                    1,  // upperLeftColumn
                    200, // height
                    300, // width
                    imagePath); // sourceFullName

                // OleObject için ek özellikleri ayarlayın
                oleObject.DisplayAsIcon = false;
                oleObject.IsAutoSize = true;

                Console.WriteLine("OLE object with linked image added successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddOleObjectWithLinkedImage method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("AddOleObjectWithLinkedImageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


