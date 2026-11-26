---
title: "Перечисление PropertyType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Properties.PropertyType. Указывает тип данных свойства документа."
type: docs
url: /ru/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

Указывает тип данных свойства документа.

```csharp
public enum PropertyType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Boolean | `0` | Свойство имеет логическое значение. |
| DateTime | `1` | Свойство имеет значение даты и времени. |
| Double | `2` | Свойство имеет число с плавающей запятой. |
| Number | `3` | Свойство имеет целочисленное значение. |
| String | `4` | Свойство имеет строковое значение. |
| Blob | `5` | Свойство имеет массив байтов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установить некоторые встроенные свойства
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Получить доступ к пользовательским свойствам документа
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Добавить пользовательские свойства разных типов
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Получить и отобразить пользовательские свойства
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Сохраните книгу
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


