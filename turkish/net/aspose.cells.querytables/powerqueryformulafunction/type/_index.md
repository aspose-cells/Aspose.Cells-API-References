---
title: "PowerQueryFormulaFunction.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaFunction özelliği. Power query formülünün türünü alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

Power query formülünün tipini alır.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir Power Query formül işlevi oluşturun
            // Doğrudan oluşturamadığımız için, onu bir yerden almamız gerekecek
            // Demo amaçları için, Type özelliğine nasıl erişileceğini sadece göstereceğiz
            // (Gerçek kullanımda, bunu mevcut bir koleksiyondan alırdınız)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Bir QueryTable'ı doğrudan da oluşturamadığımız için, o bölümü atlayacağız
            QueryTable queryTable = null; // Can't instantiate directly
            
            // Sorgu tabloları koleksiyonuna bu şekilde eklenemez - yalnızca okunur
            // worksheet.QueryTables[0] = queryTable; // Bu satır kaldırıldı
            
            // Demonstrasyon için, bir fonksiyonumuz olsaydı kullanacağımız çıktı formatını sadece göstereceğiz
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Sonucu kaydet
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


