---
title: "ShapeCollection.AddFreeform"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çalışma sayfasına serbest biçimli bir şekil ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Çalışma sayfasına serbest biçimli bir şekil ekler.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Serbest biçimli şeklin sol satırından dikey ofsetini, piksel birimi cinsinden temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Serbest biçimli şeklin sol sütunundan yatay ofsetini, piksel birimi cinsinden temsil eder. |
| yükseklik | Int32 | Serbest biçimli şeklin yüksekliğini, piksel birimi cinsinden temsil eder. |
| genişlik | Int32 | Serbest biçimli şeklin genişliğini, piksel birimi cinsinden temsil eder. |
| yollar | ShapePath[] | Kullanıcı tanımlı bir yolu temsil eder |

### Dönüş Değeri

Serbest biçimli bir şekil.

### Açıklamalar

Uyarı: Parametrelerdeki genişlik ve yükseklik, ’paths' tarafından belirtilen ShapePath dizisinin toplam genişlik ve yüksekliği değil, herhangi bir pozitif tam sayı değeri olabilir. Aralarındaki ilişki ölçek-doldurma ilişkisidir; yani her ShapePath nesnesi genişlik ve yüksekliğe göre ölçeklendirilir. Bu nedenle, 'paths' içinde birden fazla nesne olduğunda, her ShapePath nesnesi beklentileri karşılayacak şekilde makul tasarlanmalıdır. Tek bir ShapePath nesnesi olduğunda ve başka bir gereksinim bulunmadığında, nesnenin genişlik ve yüksekliğini parametre değerleri olarak geçirmek iyi bir çözümdür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Özel şekil yolları oluştur
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Çalışma sayfasına serbest biçimli şekil ekle
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Çalışma kitabını kaydedin
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


