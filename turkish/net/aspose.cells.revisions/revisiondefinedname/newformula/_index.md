---
title: "RevisionDefinedName.NewFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionDefinedName özelliği. Formülü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

Formülü alır.

```csharp
public string NewFormula { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyNewFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur ve bazı veriler ekle
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // A1'e işaret eden bir tanımlı ad ekle
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Tanımlı adı revizyon oluşturacak şekilde değiştirin (şimdi B1'e işaret ediyor)
                definedName.RefersTo = "=Sheet1!$B$1";

                // Revizyon bilgilerini gömmek için çalışma kitabını kaydedin
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // Revizyon günlüklerini okumak için çalışma kitabını yeniden açın
                Workbook revWorkbook = new Workbook(fileName);

                // Revizyonlar arasında döngü yapın ve NewFormula'yi gösterin
                foreach (RevisionLog log in revWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
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


