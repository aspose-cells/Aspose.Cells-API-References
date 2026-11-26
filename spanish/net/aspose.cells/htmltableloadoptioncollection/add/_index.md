---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método HtmlTableLoadOptionCollection. Añade un HtmlTableLoadOption a esta colección"
type: docs
url: /es/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Añade un HtmlTableLoadOption a esta colección.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | HtmlTableLoadOption | un HtmlTableLoadOption |

### Valor de retorno

el índice del elemento añadido

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método AddTableLoadOption(). Este método será eliminado 6 meses después a partir de diciembre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Agregar opciones de carga de tabla
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Cargar libro de trabajo con opciones
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Guardar la salida
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Agregar un HtmlTableLoadOption a la lista.

```csharp
public int Add(int tableIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableIndex | Int32 | Índice de tabla |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Acceder a la instancia de HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Agregar una nueva HtmlTableLoadOption por índice de tabla
            int index = tableLoadOptions.Add(0);

            // Acceder al HtmlTableLoadOption añadido
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Crear un libro de trabajo y cargar HTML con opciones
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Agregar un HtmlTableLoadOption a la lista.

```csharp
public int Add(string tableId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableId | String | ID de tabla |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Acceder a la instancia de HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Agregar una nueva HtmlTableLoadOption por id de tabla
            int index = tableLoadOptions.Add("mainTable");

            // Acceder al HtmlTableLoadOption añadido
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Crear libro de trabajo y cargar HTML con opciones
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Agregar un HtmlTableLoadOption a la lista.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableIndex | Int32 | Índice de tabla |
| targetSheetIndex | Int32 | El índice de destino de la hoja de cálculo en Excel |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Agregar tablas por índice con índice de hoja de destino
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // Cargar archivo HTML con las opciones especificadas
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Agregar un HtmlTableLoadOption a la lista.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableId | String | ID de tabla |
| targetSheetIndex | Int32 | El índice de destino de la hoja de cálculo en Excel |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Acceder a la instancia de HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Agregar una nueva HtmlTableLoadOption por id de tabla y índice de hoja de destino
            int index = tableLoadOptions.Add("tableId", 1);

            // Crear un libro de trabajo y cargar HTML con opciones
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Agregar un HtmlTableLoadOption a la lista.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableIndex | Int32 | Índice de tabla |
| targetSheetIndex | Int32 | El índice de destino de la hoja de cálculo en Excel |
| originalSheetIndex | Int32 | El índice original de la hoja de cálculo en el HTML |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Acceda a HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Agregar una tabla con índice 1, índice de hoja de destino 1, e índice de hoja original 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Crear un libro de trabajo y cargar HTML con opciones
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Agregar un HtmlTableLoadOption a la lista.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableId | String | ID de tabla |
| targetSheetIndex | Int32 | El índice de destino de la hoja de cálculo en Excel |
| originalSheetIndex | Int32 | El índice original de la hoja de cálculo en el HTML |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Demostrar el método Add con parámetros (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // Cargar archivo HTML (reemplazar con la ruta de archivo real)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


