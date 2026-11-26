---
title: "VbaProjectReferenceCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReferenceCollection. Получить ссылку в списке по индексу"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Получить ссылку из списка по индексу.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Параметр | Описание |
| --- | --- |
| i | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавить ссылки в проект VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Получить коллекцию ссылок
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Доступ к ссылкам с помощью свойства Item
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Сохраните книгу
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


