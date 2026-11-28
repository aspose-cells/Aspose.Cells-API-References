---
title: "CommentCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CommentCollection özelliği. Belirtilen indeksteki Comment öğesini alır"
type: docs
url: /tr/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Belirtilen indeksteki [`Comment`](../../comment/) öğesini alır.

```csharp
public Comment this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere yorum ekleyin
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Item özelliğini kullanarak yorumlara eriş
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Yorum notlarını ayarla
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Item özelliğini kullanarak ilk yorumu değiştir
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Yoruma koleksiyondan doğrudan eriş ve değiştir
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Çalışma kitabını kaydedin
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Belirtilen hücredeki [`Comment`](../../comment/) öğesini alır.

```csharp
public Comment this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücre adı. |

### Dönüş Değeri

Belirtilen hücredeki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücre referanslarını kullanarak hücrelere yorum ekle
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Hücre referanslarıyla Item özelliğini kullanarak yorumlara erişin
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Yorum notlarını değiştirin
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Çalışma kitabını kaydedin
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Belirtilen satır indeksi ve sütun indeksindeki [`Comment`](../../comment/) öğesini alır.

```csharp
public Comment this[int row, int column] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| satır | Satır indeksi. |
| sütun | Sütun indeksi. |

### Dönüş Değeri

Belirtilen hücredeki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücre referanslarını kullanarak hücrelere yorum ekle
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Satır/sütun indeksleriyle Item özelliğini kullanarak yorumlara erişin
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Çalışma kitabını kaydedin
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


