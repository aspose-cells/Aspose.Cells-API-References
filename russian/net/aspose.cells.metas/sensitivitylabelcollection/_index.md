---
title: "Класс SensitivityLabelCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Metas.SensitivityLabelCollection class. Представляет список меток конфиденциальности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabelcollection/
---
## SensitivityLabelCollection class

Представляет список меток чувствительности.

```csharp
public class SensitivityLabelCollection : CollectionBase<SensitivityLabel>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SensitivityLabelCollection](sensitivitylabelcollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.metas/sensitivitylabelcollection/add/)(string, bool, SensitivityLabelAssignmentType, string, SensitivityLabelMarkType) | Добавляет метку конфиденциальности. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SensitivityLabel) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SensitivityLabel, IComparer&lt;SensitivityLabel&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SensitivityLabel, IComparer&lt;SensitivityLabel&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SensitivityLabel) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SensitivityLabel[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SensitivityLabel[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SensitivityLabel[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SensitivityLabel&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр класса SensitivityLabelCollection
            SensitivityLabelCollection labels = new SensitivityLabelCollection();

            // Добавьте метки конфиденциальности с различными конфигурациями
            int index1 = labels.Add(
                id: "cb353f78-2f72-4d20-a5ca-ee47c4a5e7e1",
                isEnabled: true,
                methodType: SensitivityLabelAssignmentType.Standard,
                siteId: "contoso.sharepoint.com",
                markType: SensitivityLabelMarkType.Header);

            int index2 = labels.Add(
                id: "e48007e5-f9ac-4f63-9edc-6ab9a312688f",
                isEnabled: false,
                methodType: SensitivityLabelAssignmentType.Privileged,
                siteId: "contoso.sharepoint.com",
                markType: SensitivityLabelMarkType.Footer);

            // Примените метки к метаданным книги
            // Используем CustomDocumentProperties вместо BuiltInDocumentProperties, поскольку последние не поддерживают SensitivityLabels
            workbook.CustomDocumentProperties.Add("SensitivityLabels", labels.ToString());

            // Сохранить книгу с метками конфиденциальности
            workbook.Save("SensitivityLabelCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SensitivityLabel](../sensitivitylabel/)
* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


