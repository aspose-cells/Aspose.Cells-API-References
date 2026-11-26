---
title: "CustomDocumentPropertyCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomDocumentPropertyCollection. Crea una nueva propiedad de documento personalizada del tipo de datos PropertyType.String"
type: docs
url: /es/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| valor | String | El valor de la propiedad. |

### Valor de retorno

El objeto de propiedad recién creado.

### Ejemplos

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

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| valor | Int32 | El valor de la propiedad. |

### Valor de retorno

El objeto de propiedad recién creado.

### Ejemplos

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
            
            // Agregar propiedades de documento personalizadas
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar las propiedades
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| valor | DateTime | El valor de la propiedad. |

### Valor de retorno

El objeto de propiedad recién creado.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la colección de propiedades de documento personalizadas
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // Agregar una propiedad DateTime
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // Mostrar información sobre la propiedad agregada
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // Guardar el libro de trabajo (opcional, demuestra que la propiedad persiste)
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

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| valor | Booleano | El valor de la propiedad. |

### Valor de retorno

El objeto de propiedad recién creado.

### Ejemplos

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

            // Agregar una propiedad personalizada booleana
            customProperties.Add("IsApproved", true);

            // Mostrar la propiedad agregada
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // Guarda el libro de trabajo
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| valor | Double | El valor de la propiedad. |

### Valor de retorno

El objeto de propiedad recién creado.

### Ejemplos

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

            // Demostrar el método Add con parámetros String y Double
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // Acceder y mostrar las propiedades agregadas
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


