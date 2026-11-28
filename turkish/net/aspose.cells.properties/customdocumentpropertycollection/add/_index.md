---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomDocumentPropertyCollection yöntemi. PropertyType.String veri tipinde yeni bir özel belge özelliği oluşturur"
type: docs
url: /tr/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

**PropertyType.String** veri tipinde yeni bir özel belge özelliği oluşturur.

```csharp
public DocumentProperty Add(string name, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| değer | String | Özelliğin değeri. |

### Dönüş Değeri

Yeni oluşturulan özelliğin nesnesi.

### Örnekler

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

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

**PropertyType.Number** veri tipinde yeni bir özel belge özelliği oluşturur.

```csharp
public DocumentProperty Add(string name, int value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| değer | Int32 | Özelliğin değeri. |

### Dönüş Değeri

Yeni oluşturulan özelliğin nesnesi.

### Örnekler

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
            
            // Özel belge özellikleri ekle
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Özellikleri doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

**PropertyType.DateTime** veri tipinde yeni bir özel belge özelliği oluşturur.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| değer | DateTime | Özelliğin değeri. |

### Dönüş Değeri

Yeni oluşturulan özelliğin nesnesi.

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Özel belge özellikleri koleksiyonunu al
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Bir DateTime özelliği ekle
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Eklenen özellik hakkında bilgi göster
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Çalışma kitabını kaydet (isteğe bağlı, özelliğin kalıcı olduğunu gösterir)
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

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

**PropertyType.Boolean** veri tipinde yeni bir özel belge özelliği oluşturur.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| değer | Boolean | Özelliğin değeri. |

### Dönüş Değeri

Yeni oluşturulan özelliğin nesnesi.

### Örnekler

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

            // Boolean özel özelliği ekle
            customProperties.Add("IsApproved", true);

            // Eklenen özelliği göster
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Çalışma kitabını kaydedin
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

**PropertyType.Float** veri tipinde yeni bir özel belge özelliği oluşturur.

```csharp
public DocumentProperty Add(string name, double value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| değer | Double | Özelliğin değeri. |

### Dönüş Değeri

Yeni oluşturulan özelliğin nesnesi.

### Örnekler

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

            // String ve Double parametrelerle Add metodunu göster
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Eklenen özelliklere eriş ve göster
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


