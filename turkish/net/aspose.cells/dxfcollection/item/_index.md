---
title: "DxfCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DxfCollection özelliği. Belirtilen indeksteki öğeyi alır"
type: docs
url: /tr/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Belirtilen indeksteki öğeyi alır.

```csharp
public Style this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Belirtilen indeks. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // DxfCollection'a çalışma kitabından erişin
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Yeni bir stil oluştur (DxfCollection'a doğrudan eklenemez çünkü Add yöntemi yoktur)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // Stil oluşturulduğunda otomatik olarak koleksiyona eklenir

            // Item özelliğini kullanarak DxfCollection'dan ilk öğeyi al
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Stili Item özelliği üzerinden değiştirin (çünkü bir referans döndürür)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Değişikliği doğrulayın
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Stili bir hücreye uygulayarak etkisini görün
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Sonucu kaydet
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


