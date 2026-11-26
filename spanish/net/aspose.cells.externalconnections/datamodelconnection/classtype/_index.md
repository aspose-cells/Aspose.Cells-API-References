---
title: "DataModelConnection.ClassType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelConnection. Obtiene el tipo de este objeto ExternalConnection"
type: docs
url: /es/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

Obtiene el tipo de este objeto [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear una instancia de DataModelConnection usando un objeto no inicializado
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // Mostrar el valor actual de ClassType (propiedad de solo lectura)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // Configurar propiedades de conexión
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // Demostrar cómo ClassType afecta el manejo de la conexión
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // Agregar PowerQueryFormula para la conexión del modelo de datos
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // Guarda el libro de trabajo
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


