---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomDocumentPropertyCollection method. Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp PropertyType.String"
type: docs
url: /de/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| Wert | String | Der Wert der Eigenschaft. |

### Rückgabewert

Das neu erstellte Eigenschaftsobjekt.

### Beispiele

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

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| Wert | Int32 | Der Wert der Eigenschaft. |

### Rückgabewert

Das neu erstellte Eigenschaftsobjekt.

### Beispiele

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
            
            // Benutzerdefinierte Dokumenteigenschaften hinzufügen
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen Sie die Eigenschaften
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| Wert | DateTime | Der Wert der Eigenschaft. |

### Rückgabewert

Das neu erstellte Eigenschaftsobjekt.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Hole die Sammlung benutzerdefinierter Dokumenteigenschaften
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Fügen Sie eine DateTime-Eigenschaft hinzu
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Zeigen Sie Informationen über die hinzugefügte Eigenschaft an
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Speichern Sie die Arbeitsmappe (optional, zeigt, dass die Eigenschaft erhalten bleibt)
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

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| Wert | Boolean | Der Wert der Eigenschaft. |

### Rückgabewert

Das neu erstellte Eigenschaftsobjekt.

### Beispiele

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

            // Fügen Sie eine boolesche benutzerdefinierte Eigenschaft hinzu
            customProperties.Add("IsApproved", true);

            // Zeigen Sie die hinzugefügte Eigenschaft an
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Speichere die Arbeitsmappe
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Erstellt eine neue benutzerdefinierte Dokumenteigenschaft vom Datentyp **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Eigenschaft. |
| Wert | Double | Der Wert der Eigenschaft. |

### Rückgabewert

Das neu erstellte Eigenschaftsobjekt.

### Beispiele

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

            // Demonstrieren Sie die Add-Methode mit String- und Double-Parametern
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Greifen Sie auf die hinzugefügten Eigenschaften zu und zeigen Sie sie an
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### Siehe auch

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


