---
title: "RevisionDefinedName.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionDefinedName özelliği. Tanımlı adın metnini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Tanımlı adın metnini alır.

```csharp
public string Text { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionDefinedNamePropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Tanımlı bir ad oluşturun
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Revizyon oluşturacak şekilde tanımlı adı değiştirin
            name.RefersTo = "=Sheet1!$B$1";
            
            // Revizyonlar oluşturmak için dosyaya kaydedin
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Revizyonları okumak için dosyayı yeniden açın
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Revizyonları kontrol edin
            foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.DefinedName)
                    {
                        RevisionDefinedName rdn = (RevisionDefinedName)rv;
                        Console.WriteLine("Defined Name Text: " + rdn.Text);
                        Console.WriteLine("Old Formula: " + rdn.OldFormula);
                        Console.WriteLine("New Formula: " + rdn.NewFormula);
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


