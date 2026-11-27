---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomDocumentPropertyCollection metod. Skapar en ny anpassad dokumentegenskap av datatypen PropertyType.String"
type: docs
url: /sv/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| värde | String | Värdet på egenskapen. |

### Returvärde

Det nyss skapade egenskapsobjektet.

### Exempel

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

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| värde | Int32 | Värdet på egenskapen. |

### Returvärde

Det nyss skapade egenskapsobjektet.

### Exempel

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
            
            // Lägg till anpassade dokumentegenskaper
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| värde | DateTime | Värdet på egenskapen. |

### Returvärde

Det nyss skapade egenskapsobjektet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta samlingen av anpassade dokumentegenskaper
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Lägg till en DateTime-egenskap
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Visa information om den tillagda egenskapen
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Spara arbetsboken (valfritt, demonstrerar att egenskapen kvarstår)
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

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| värde | Boolean | Värdet på egenskapen. |

### Returvärde

Det nyss skapade egenskapsobjektet.

### Exempel

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

            // Lägg till en boolesk anpassad egenskap
            customProperties.Add("IsApproved", true);

            // Visa den tillagda egenskapen
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Spara arbetsboken
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på egenskapen. |
| värde | Double | Värdet på egenskapen. |

### Returvärde

Det nyss skapade egenskapsobjektet.

### Exempel

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

            // Demonstrera Add-metoden med String- och Double-parametrar
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Kom åt och visa de tillagda egenskaperna
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### Se även

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


