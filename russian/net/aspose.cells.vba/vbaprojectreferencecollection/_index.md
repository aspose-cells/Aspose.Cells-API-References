---
title: "Класс VbaProjectReferenceCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Vba.VbaProjectReferenceCollection. Представляет все ссылки VBA‑проекта"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Представляет все ссылки проекта VBA.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item/) { get; } | Получить ссылку из списка по индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [AddControlReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolreferernce/)(string, string, string, string) | Добавить ссылку на изменённую типовую библиотеку и её расширенную типовую библиотеку. |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/)(string, string, string, string) | (**Obsolete.**) Добавить ссылку на изменённую типовую библиотеку и её расширенную типовую библиотеку. |
| [AddProjectReferernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectreferernce/)(string, string, string) | Добавляет ссылку на внешний VBA‑проект. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/)(string, string, string) | (**Obsolete.**) Добавляет ссылку на внешний VBA‑проект. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/)(string, string) | Добавить ссылку на типовую библиотеку Automation. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy/)(VbaProjectReferenceCollection) | Копирует ссылки из другого VBA‑проекта. |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaProjectReference[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaProjectReference[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VbaProjectReference[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaProjectReference) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaProjectReference, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaProjectReference, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaProjectReference) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaProjectReference, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaProjectReference, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceCollectionDemo
    {
        public static void VbaProjectReferenceCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавить ссылку на проект VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Добавить ещё одну ссылку на VBA‑проект
            vbaProject.References.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "twiddledLibid", "extendedLibid");
            
            // Добавить ссылку на проект
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Доступ к коллекции ссылок
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Отображение количества ссылок
            Console.WriteLine("Total References: " + references.Count);
            
            // Доступ к конкретной ссылке
            VbaProjectReference reference = references[0];
            Console.WriteLine("First Reference Name: " + reference.Name);
            
            // Копирование ссылок из другой коллекции (предполагая, что anotherVbaProjectReferences — это другой VbaProjectReferenceCollection)
            // VbaProjectReferenceCollection anotherVbaProjectReferences = ...;
            // references.Copy(anotherVbaProjectReferences);
            
            // Сохранение файла Excel
            workbook.Save("VbaProjectReferenceCollectionExample.xlsm");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaProjectReference](../vbaprojectreference/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


