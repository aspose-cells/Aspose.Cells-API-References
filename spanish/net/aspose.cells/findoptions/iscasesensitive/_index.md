---
title: "FindOptions.IsCaseSensitive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Indica si la cadena buscada distingue mayúsculas y minúsculas"
type: docs
url: /es/net/aspose.cells/findoptions/iscasesensitive/
---
## FindOptions.IsCaseSensitive property

Indica si la cadena buscada distingue entre mayúsculas y minúsculas.

```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FindOptions.CaseSensitive. Esta propiedad será eliminada 12 meses después desde junio de 2010. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyIsCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("AbC");

            FindOptions options = new FindOptions();
            options.IsCaseSensitive = true;
            
            // Buscar coincidencia sensible a mayúsculas
            Cell cell = worksheet.Cells.Find("abc", null, options);
            
            Console.WriteLine("Case-sensitive search for 'abc' found at: " + 
                              (cell != null ? cell.Name : "No match"));
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


