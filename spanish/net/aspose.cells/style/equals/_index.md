---
title: "Style.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Determina si dos instancias de Style son iguales"
type: docs
url: /es/net/aspose.cells/style/equals/
---
## Style.Equals method

Determina si dos instancias de Style son iguales.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto Style para comparar con el objeto Style actual. |

### Valor de retorno

true si el Objeto especificado es igual al Objeto actual; de lo contrario, false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos estilos para comparar
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Llamar al método Equals para comparar los estilos
                bool areEqual = style1.Equals((object)style2);

                // Mostrar el resultado
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Aplicar los estilos para demostrar que son idénticos
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


