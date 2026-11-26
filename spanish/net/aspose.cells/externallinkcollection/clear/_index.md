---
title: "ExternalLinkCollection.Clear"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExternalLinkCollection. Elimina todos los enlaces externos"
type: docs
url: /es/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Elimina todos los enlaces externos.

```csharp
public void Clear()
```

### Observaciones

Al eliminar enlaces externos, todas las fórmulas que hacen referencia a ellos también se eliminarán porque las referencias se vuelven inválidas.

### Ver también

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Elimina todos los enlaces externos.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| updateReferencesAsLocal | Booleano | Indica si se actualizan todas las referencias de enlaces externos en las fórmulas a referencias del propio libro de trabajo actual. |

### Observaciones

Si se requiere actualizar las referencias, esas referencias de enlaces externos en las fórmulas se cambiarán al libro de trabajo actual cuando sea posible. Por ejemplo, la fórmula original de una celda es "='externalsource.xlam'!customfunction()", después de eliminar los enlaces externos, la fórmula se convertirá en "=customfunction()"; Cuando la fórmula original es "='[externalsource.xlam]Sheet1'!$A$1", según exista una hoja con el nombre "Sheet1" en el libro de trabajo actual: si es verdadero, la fórmula se convertirá en "=Sheet1!$A$1"; si es falso, la fórmula se convertirá en "=#REF!$A$1". Si no se requiere actualizar las referencias, todas las fórmulas con referencias a enlaces externos también se eliminarán porque esas referencias se vuelven inválidas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos enlaces externos
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // Limpiar con updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Agregar enlaces nuevamente
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // Limpiar con updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### Ver también

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


