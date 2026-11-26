---
title: "RevisionDefinedName.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionDefinedName. Получает текст определённого имени"
type: docs
url: /ru/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Получает текст определённого имени.

```csharp
public string Text { get; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте определённое имя
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Измените определённое имя, чтобы создать ревизию
            name.RefersTo = "=Sheet1!$B$1";
            
            // Сохраните в файл, чтобы создать ревизии
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Откройте файл снова, чтобы прочитать ревизии
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Проверьте ревизии
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

### См. также

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


