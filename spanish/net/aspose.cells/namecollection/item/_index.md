---
title: "NameCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NameCollection. Obtiene el elemento Name en el índice especificado"
type: docs
url: /es/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Obtiene el elemento [`Name`](../../name/) en el índice especificado.

```csharp
public Name this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Acceder a la colección de nombres
            NameCollection names = workbook.Worksheets.Names;
            
            // Agregar rangos con nombre usando la firma de método correcta
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Demostrar el uso de la propiedad Item
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Acceder por nombre usando la propiedad Item
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Modificar un rango con nombre
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### Ver también

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Obtiene el elemento [`Name`](../../name/) con el nombre especificado.

```csharp
public Name this[string text] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| texto | Texto del nombre. |

### Valor de retorno

El elemento con el nombre especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la colección de nombres de las hojas de cálculo
            NameCollection names = workbook.Worksheets.Names;
            
            // Agregar algunos rangos con nombre (corregido para usar la firma adecuada del método Add)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Acceder a los rangos con nombre usando la propiedad Item
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Verificar que los nombres existan
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Intentar acceder a un nombre inexistente
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### Ver también

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


