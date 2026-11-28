---
title: "RevisionDefinedName.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionDefinedName özelliği. Revizyonun türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Revizyonun türünü temsil eder.

```csharp
public override RevisionType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluşturun ve tanımlı bir ad ekleyin
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Revizyon kaydı oluşturacak şekilde tanımlı adı değiştirin
                definedName.RefersTo = "=Sheet1!$B$1";

                // Revizyon bilgilerini gömmek için çalışma kitabını kaydedin
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Revizyon günlüğünü okumak için çalışma kitabını yeniden açın
                Workbook revWb = new Workbook(filePath);

                // Revizyonlar arasında döngü yapın ve her RevisionDefinedName girişinin Type'ını gösterin
                foreach (RevisionLog log in revWb.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Revision Type: {rdn.Type}");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


