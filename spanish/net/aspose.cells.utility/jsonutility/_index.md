---
title: "Clase JsonUtility"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Utility.JsonUtility. Representa la clase de utilidad para procesar json"
type: docs
url: /es/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

Representa la clase de utilidad para procesar JSON.

```csharp
public class JsonUtility
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [JsonUtility](jsonutility/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Exportando el rango a un archivo json. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Exportando el rango a un archivo json. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Importar la cadena json. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // Crear una instancia de JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // Dado que la clase JsonUtility no tiene ninguna propiedad o método definido en el JSON,
            // demostraremos su instanciación y uso potencial de forma contextual.

            // Ejemplo: Suponiendo que JsonUtility podría usarse para procesar datos JSON de alguna manera.
            // Nota: El uso real dependería de los métodos y propiedades disponibles en la clase real.
            // Aquí solo estamos demostrando la instanciación ya que no se proporcionan métodos ni propiedades.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Código adicional para demostrar el uso potencial
            // Por ejemplo, si JsonUtility tuviera un método para procesar JSON, podría verse así:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Dado que no se proporcionan métodos, terminaremos el ejemplo aquí.
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


