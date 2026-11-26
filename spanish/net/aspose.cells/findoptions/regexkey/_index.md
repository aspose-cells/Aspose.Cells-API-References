---
title: "FindOptions.RegexKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Indica si la clave buscada es una expresión regular. Si es true, la clave buscada se tomará como expresión regular y se analizará. De lo contrario, la clave se analizará según las reglas de MS Excel"
type: docs
url: /es/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Indica si la clave buscada es una expresión regular. Si es verdadero, la clave buscada se tomará como expresión regular y se analizará. De lo contrario, la clave se analizará según las reglas de MS Excel.

```csharp
public bool RegexKey { get; set; }
```

### Observaciones

Aunque la clave de búsqueda se haya especificado como expresión regular, puede ser reformulada según el [`LookAtType`](../lookattype/) especificado. Por ejemplo, cuando el tipo es Contains (este es el valor predeterminado para estas opciones), se agregarán comodines al principio y al final de la clave de búsqueda automáticamente para asegurar que la coincidencia se verifique como \"contains\". En este caso, las expresiones regulares se volverán más complejas y el rendimiento también disminuirá. Por lo tanto, por consideraciones de rendimiento, si el usuario ha especificado la regla exacta para la expresión regular, no es necesario usar [`LookAtType`](../lookattype/) como restricción adicional y el usuario puede establecerlo como EntireContent para obtener mejor rendimiento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de prueba con cadenas que coincidan con patrones
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Crear opciones de búsqueda con regex habilitado
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Buscar celdas que coincidan con el patrón regex
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Mostrar el resultado
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


