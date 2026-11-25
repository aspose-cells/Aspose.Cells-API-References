---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomDocumentPropertyCollection. Crea una nuova proprietà personalizzata del documento del tipo di dati PropertyType.String"
type: docs
url: /it/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| valore | String | Il valore della proprietà. |

### Valore di ritorno

L'oggetto proprietà appena creato.

### Esempi

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

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| valore | Int32 | Il valore della proprietà. |

### Valore di ritorno

L'oggetto proprietà appena creato.

### Esempi

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
            
            // Aggiungi proprietà di documento personalizzate
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica le proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| valore | DateTime | Il valore della proprietà. |

### Valore di ritorno

L'oggetto proprietà appena creato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Ottieni la collezione delle proprietà del documento personalizzate
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Aggiungi una proprietà DateTime
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Visualizza le informazioni sulla proprietà aggiunta
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Salva la cartella di lavoro (opzionale, dimostra che la proprietà persiste)
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

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| valore | Booleano | Il valore della proprietà. |

### Valore di ritorno

L'oggetto proprietà appena creato.

### Esempi

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

            // Aggiungi una proprietà personalizzata booleana
            customProperties.Add("IsApproved", true);

            // Visualizza la proprietà aggiunta
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Salva la cartella di lavoro
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Crea una nuova proprietà di documento personalizzata del tipo di dati **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà. |
| valore | Double | Il valore della proprietà. |

### Valore di ritorno

L'oggetto proprietà appena creato.

### Esempi

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

            // Dimostra il metodo Add con parametri String e Double
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Accedi e visualizza le proprietà aggiunte
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


