---
title: "FunctionEquationNode.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FunctionEquationNode. Determinar si el nodo de ecuación actual es igual al nodo especificado"
type: docs
url: /es/net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Determinar si el nodo de ecuación actual es igual al nodo especificado

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El nodo especificado |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FunctionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma TextBox para contener una ecuación
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 200, 100);

            // Obtener el nodo raíz de la ecuación del TextBox
            EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

            // Crear el primer nodo de ecuación de función
            FunctionEquationNode funcNode1 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            // (Opcional) Agregar contenido mínimo para que el nodo sea válido
            EquationNode funcName1 = funcNode1.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText1 = (TextRunEquationNode)funcName1.AddChild(EquationNodeType.Text);
            nameText1.Text = "Sin";

            // Crear el segundo nodo de ecuación de función
            FunctionEquationNode funcNode2 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            EquationNode funcName2 = funcNode2.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText2 = (TextRunEquationNode)funcName2.AddChild(EquationNodeType.Text);
            nameText2.Text = "Cos";

            try
            {
                // Comparar los dos nodos de función usando Equals(Object)
                bool areEqual = funcNode1.Equals((object)funcNode2);
                Console.WriteLine($"funcNode1.Equals(funcNode2) returned: {areEqual}");

                // Comparar un nodo consigo mismo
                bool selfEqual = funcNode1.Equals((object)funcNode1);
                Console.WriteLine($"funcNode1.Equals(funcNode1) returned: {selfEqual}");

                // Guardar el libro de trabajo (no se necesitan cambios visuales para esta demostración)
                workbook.Save("FunctionEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


