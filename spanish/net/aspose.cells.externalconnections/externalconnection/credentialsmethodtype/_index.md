---
title: "ExternalConnection.CredentialsMethodType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica el método de autenticación que se utilizará al establecer o restablecer la conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

Especifica el método de autenticación que se debe usar al establecer (o restablecer) la conexión.

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Agregue una hoja de cálculo y cree una tabla dinámica para establecer una conexión externa
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // Cree una tabla dinámica que tendrá una conexión externa
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // Obtenga la conexión externa de la tabla dinámica
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Muestre el valor actual de CredentialsMethodType
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // Demuestre la configuración de la propiedad (ya que es de lectura-escritura)
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // Establezca otro valor para demostrar
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


