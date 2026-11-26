---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomDocumentPropertyCollection. Создаёт новое пользовательское свойство документа типа данных PropertyType.String"
type: docs
url: /ru/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Создаёт новое пользовательское свойство документа типа данных **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| значение | String | Значение свойства. |

### Возвращаемое значение

Недавно созданный объект свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.CustomDocumentProperties.Add("startdate", "ToneyTest");
            
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["startdate"].Value);
                
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Создаёт новое пользовательское свойство документа типа данных **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| значение | Int32 | Значение свойства. |

### Возвращаемое значение

Недавно созданный объект свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet1");
            
            // Добавить пользовательские свойства документа
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверьте свойства
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Создаёт новое пользовательское свойство документа типа данных **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| значение | DateTime | Значение свойства. |

### Возвращаемое значение

Недавно созданный объект свойства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Properties;

    public class CustomDocumentPropertyCollectionMethodAddWithStringDateTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить коллекцию пользовательских свойств документа
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Добавьте свойство DateTime
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Отобразите информацию о добавленном свойстве
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Сохраните книгу (необязательно, демонстрирует, что свойство сохраняется)
                workbook.Save("AddDateTimePropertyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding DateTime property: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Создаёт новое пользовательское свойство документа типа данных **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| значение | Boolean | Значение свойства. |

### Возвращаемое значение

Недавно созданный объект свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Добавьте пользовательское булево свойство
            customProperties.Add("IsApproved", true);

            // Отобразите добавленное свойство
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Сохраните книгу
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Создаёт новое пользовательское свойство документа типа данных **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| значение | Double | Значение свойства. |

### Возвращаемое значение

Недавно созданный объект свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Продемонстрируйте метод Add с параметрами String и Double
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Получите доступ и отобразите добавленные свойства
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


