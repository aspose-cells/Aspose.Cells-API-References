---
title: "RevisionInsertSheet.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertSheet özelliği. Çalışma sayfasının adını alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Eski formülü alır.

```csharp
public string OldFormula { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionDefinedNamePropertyOldFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Revizyon geçmişi oluşturmak için tanımlı bir ad ekleyin
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Bir revizyon oluşturmak için tanımlı adı değiştir
                definedName.RefersTo = "=Sheet1!$B$1";

                // Revizyonları kalıcı kılmak için çalışma kitabını kaydedin
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Revizyon günlüklerine erişmek için çalışma kitabını yeniden aç
                Workbook revisionWorkbook = new Workbook(filePath);

                // Tanımlı ad revizyonlarını bulmak için revizyon günlükleri arasında döngü yapın
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;
                            Console.WriteLine("Defined Name Text: " + revisionDefinedName.Text);
                            Console.WriteLine("Old Formula: " + revisionDefinedName.OldFormula);
                            Console.WriteLine("New Formula: " + revisionDefinedName.NewFormula);
                        }
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


