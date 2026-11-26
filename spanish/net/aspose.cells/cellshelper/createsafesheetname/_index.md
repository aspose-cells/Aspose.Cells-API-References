---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán con   y luego se devolverá el valor de cadena reconstruido."
type: docs
url: /es/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán por ' ', luego se devuelve el valor de cadena reconstruido.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nameProposal | String | nombre de hoja a usar |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán por el carácter especificado, luego se devuelve el valor de cadena reconstruido.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nameProposal | String | nombre de hoja a usar |
| replaceChar | Carácter | carácter que se utilizará para reemplazar caracteres inválidos en el nombre de hoja dado |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Ejemplo 1: Crear un nombre de hoja seguro con el carácter de reemplazo predeterminado
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Ejemplo 2: Crear un nombre de hoja seguro con el carácter de reemplazo personalizado 'A'
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


