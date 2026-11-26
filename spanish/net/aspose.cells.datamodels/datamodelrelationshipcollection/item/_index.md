---
title: "DataModelRelationshipCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelRelationshipCollection. Obtiene la relación"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Obtiene la relación.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo (modelo de datos vacío)
            Workbook workbook = new Workbook();

            try
            {
                // Obtener la DataModelRelationshipCollection del libro de trabajo (puede ser nula si no hay modelo de datos)
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // Leer la primera relación usando la propiedad Item (indexador)
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Guardar el libro de trabajo (opcional, solo para demostrar que el código se ejecuta de extremo a extremo)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


