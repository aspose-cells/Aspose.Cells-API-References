---
title: "Класс WorkbookMetadata"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Metadata.WorkbookMetadata. Представляет метаданные"
type: docs
url: /ru/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

Представляет метаданные.

```csharp
public class WorkbookMetadata
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | Создайте объект метаданных. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | Создайте объект метаданных. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | Возвращает коллекцию [`DocumentProperty`](../../aspose.cells.properties/documentproperty/), представляющую все встроенные свойства документа таблицы. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | Возвращает коллекцию [`DocumentProperty`](../../aspose.cells.properties/documentproperty/), представляющую все пользовательские свойства документа таблицы. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | Получает параметры метаданных. |

## Методы

| Имя | Описание |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | Сохраните изменённые метаданные в поток. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | Сохраните изменённые метаданные в файл. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class WorkbookMetadataDemo
    {
        public static void WorkbookMetadataExample()
        {
            // Создайте экземпляр MetadataOptions
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // Создайте экземпляр WorkbookMetadata с именем файла и параметрами
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // Добавьте пользовательское свойство документа
            meta.CustomDocumentProperties.Add("test", "test");

            // Сохраните метаданные в новый файл
            meta.Save("WorkbookMetadataExample.xlsx");

            // Продемонстрируйте доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // Продемонстрируйте доступ к пользовательским свойствам документа
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // Сохраните метаданные в поток
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


