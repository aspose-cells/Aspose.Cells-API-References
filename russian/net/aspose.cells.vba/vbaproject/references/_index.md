---
title: "VbaProject.References"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Получает все ссылки VBA проекта"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Получает все ссылки проекта VBA.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // Создать книгу (VBA проект создаётся автоматически для файлов .xlsm)
            Workbook workbook = new Workbook();
            
            // Получить доступ к ссылкам VBA проекта (доступно только если книга содержит VBA проект)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Добавить различные типы ссылок
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Отобразить количество ссылок
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Сохранить как книгу с поддержкой макросов
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### См. также

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


