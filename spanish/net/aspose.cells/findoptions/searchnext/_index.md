---
title: "FindOptions.SearchNext"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FindOptions. Orden de búsqueda. True busca siguiente. False busca anterior"
type: docs
url: /es/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

Orden de búsqueda. True: buscar siguiente. False: buscar anterior.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FindOptions.SearchBackward. Esta propiedad será eliminada 12 meses después desde noviembre de 2018. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // Crear opciones de búsqueda
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // Demostrar la propiedad SearchNext (obsoleta, pero mostrada para demostración)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // Buscar hacia adelante (comportamiento predeterminado)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // Buscar hacia atrás
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // Guarda el libro de trabajo
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


