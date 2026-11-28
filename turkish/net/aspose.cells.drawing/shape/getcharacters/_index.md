---
title: "Shape.GetCharacters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Metin içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Metin içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Dönüş Değeri

Tüm Characters nesneleri

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Shape.GetRichFormattings() yöntemini kullanın. Bu yöntem, Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle çalışma sayfasına bir metin kutusu şekli ekleyin
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Şekilden karakterleri alın
            ArrayList characters = shape.GetCharacters();

            // Her karakter hakkında bilgiyi gösterin
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


