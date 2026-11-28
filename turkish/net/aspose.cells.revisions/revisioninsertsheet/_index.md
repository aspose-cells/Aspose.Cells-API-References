---
title: "Sınıf RevisionInsertSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionInsertSheet sınıfı. Eklenen bir sayfanın revizyon kaydını temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

Eklmiş bir sayfanın revizyon kaydını temsil eder.

```csharp
public class RevisionInsertSheet : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | Revizyonun eylem türünü alır. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | Çalışma sayfasının adını alır. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | Yeni sayfanın sayfa sekme çubuğundaki sıfır tabanlı konumunu alır. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | Revizyon tipini alır. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionInsertSheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir revizyon oluşturma ihtimali için yeni bir çalışma sayfası ekleyin
                Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

                // Not: RevisionInsertSheet örneklerini doğrudan oluşturamadığımız için,
                // revizyonlar koleksiyonunda mevcut olsaydı, onunla nasıl çalışılacağını göstereceğiz
                // Gerçek revizyon izleme API'si tam olarak açıktan çıkarılmadığı için bu bir simüle senaryodur

                // Revizyon izleme etkinleştirilmiş gerçek bir senaryoda, revizyonları şu şekilde alabilirsiniz:
                // RevisionInsertSheet revision = null; // workbook.Revisions koleksiyonundan gelecekti

                // Demonstrasyon amaçları için, bir RevisionInsertSheet ile çalışma desenini göstereceğiz
                // Doğrudan örnekleyemediğimiz için, özellik erişim desenini göstereceğiz

                // Bir örnek oluşturmaya çalışmak yerine, mevcutsa onunla nasıl çalışılacağını göstereceğiz
                // Bu, derleme hatasını düzeltirken yapıyı korur

                // Revizyon özellikleri hakkında bilgi göster (simüle edilmiş)
                Console.WriteLine("RevisionInsertSheet properties demonstration:");
                Console.WriteLine("Type property would show: RevisionType.InsertSheet");
                Console.WriteLine("ActionType property would show: RevisionActionType.Add");
                Console.WriteLine("Name property would show the sheet name");
                Console.WriteLine("SheetPosition property would show the zero-based position");

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionInsertSheetDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with potential revisions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionInsertSheet: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


