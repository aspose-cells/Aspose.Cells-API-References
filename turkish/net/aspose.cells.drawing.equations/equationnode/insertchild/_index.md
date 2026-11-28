---
title: "EquationNode.InsertChild"
second_title: "Aspose.Cells için .NET API Referansı"
description: "EquationNode yöntemi. Belirtilen türde bir düğümü, mevcut düğümlerin alt düğüm listesinde belirtilen indeks konumuna ekler"
type: docs
url: /tr/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Belirtilen tipte bir düğümü geçerli düğümün alt düğüm listesindeki belirtilen indeks konumuna ekler.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | indeks değeri |
| equationType | EquationNodeType | Denklem Düğümlerinin Türleri |

### Dönüş Değeri

Belirtilen tür mevcutsa, karşılık gelen düğüm döndürülür; tür mevcut değilse, bilinmeyen türde bir düğüm döndürülür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir denklem şekli oluştur
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Denkleme başlangıç metin düğümünü ekle
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // İndeks 0'da yeni bir kesir düğümü ekle
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Çalışma kitabını kaydedin
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


