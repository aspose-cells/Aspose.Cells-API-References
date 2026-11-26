---
title: "DelimiterEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DelimiterEquationNode. Determinar si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/delimiterequationnode/equals/
---
## DelimiterEquationNode.Equals method

Determinar si el nodo de ecuación actual es igual al nodo especificado

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El nodo especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class DelimiterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos instancias de DelimiterEquationNode para comparación
            // Dado que DelimiterEquationNode no tiene un constructor sin parámetros,
            // necesitaremos crearlos de manera diferente. Suponiendo que podamos usar el constructor predeterminado
            // de la clase base o encontrar otra forma de crearlos.
            // Para la demostración, utilizaremos ObjectCreationHelper (hipotético) o un enfoque similar
            DelimiterEquationNode node1 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node1.BeginChar = "(";
            node1.EndChar = ")";
            node1.SeparatorChar = ",";
            node1.DelimiterShape = EquationDelimiterShapeType.Centered;

            DelimiterEquationNode node2 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node2.BeginChar = "(";
            node2.EndChar = ")";
            node2.SeparatorChar = ",";
            node2.DelimiterShape = EquationDelimiterShapeType.Centered;

            try
            {
                // Llamar al método Equals con el parámetro Object
                bool result = node1.Equals((Object)node2);

                // Mostrar el resultado
                Console.WriteLine($"Equals method result: {result}");

                // Modificar node2 para que sean diferentes
                node2.BeginChar = "[";
                bool result2 = node1.Equals((Object)node2);
                Console.WriteLine($"Equals method result after modification: {result2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("DelimiterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


