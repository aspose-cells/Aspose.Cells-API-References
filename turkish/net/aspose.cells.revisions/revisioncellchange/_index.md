---
title: "Sınıf RevisionCellChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionCellChange sınıfı. Hücreleri değiştiren revizyonu temsil eder."
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Hücreleri değiştiren revizyonu temsil eder.

```csharp
public class RevisionCellChange : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Hücrenin adını alır. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Hücrenin sütun indeksini alır. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Bu hücrenin yeni biçimlendirilip biçimlendirilmediğini gösterir. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Bu hücrenin eski biçimlendirilip biçimlendirilmediğini gösterir. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Eski formülü alır. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Hücrenin yeni stilini alır. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Hücrenin yeni değerini alır. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Eski formülü alır. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Hücrenin eski stilini alır. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Hücrenin eski değerini alır. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Hücrenin satır indeksini alır. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Revizyonun türünü temsil eder. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // Çıktı dizini yoksa oluştur
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // İlk çalışma kitabını oluştur ve paylaşımı etkinleştir
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // İzlenen değişiklikler yapmak için çalışma kitabını yeniden aç
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // İlk revizyon: İlk değerleri ayarla
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // İkinci revizyon: Değerleri değiştir
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Revizyon günlüklerine erişmek için çalışma kitabını yükle
            Workbook workbook3 = new Workbook(filePath);
            
            // Tüm revizyon günlüklerini işle
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


