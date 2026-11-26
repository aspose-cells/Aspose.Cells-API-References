---
title: "RevisionInsertSheet.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertSheet. Получает имя листа"
type: docs
url: /ru/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Получает старую формулу.

```csharp
public string OldFormula { get; }
```

### Примеры

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
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте определённое имя, чтобы создать историю ревизий
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Изменить определённое имя для создания ревизии
                definedName.RefersTo = "=Sheet1!$B$1";

                // Сохраните книгу, чтобы сохранить ревизии
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Повторно открыть книгу, чтобы получить доступ к журналам ревизий
                Workbook revisionWorkbook = new Workbook(filePath);

                // Пройдите по журналам ревизий, чтобы найти ревизии определённых имён
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

### См. также

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


