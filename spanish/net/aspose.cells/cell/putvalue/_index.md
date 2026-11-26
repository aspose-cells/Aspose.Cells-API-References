---
title: "Cell.PutValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Cell. Inserta un valor booleano en la celda"
type: docs
url: /es/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Coloca un valor booleano en la celda.

```csharp
public void PutValue(bool boolValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| boolValue | Booleano |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Insertar un valor booleano en la celda B3 (fila 2, columna 2)
            cells[2, 2].PutValue(true);

            // Verificar que el valor se haya establecido correctamente
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Coloca un valor entero en la celda.

```csharp
public void PutValue(int intValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intValue | Int32 | Valor de entrada |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Usando PutValue con parámetros Int32
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Calcular la suma de los valores
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Coloca un valor double en la celda.

```csharp
public void PutValue(double doubleValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleValue | Double | Valor de entrada |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Insertar valores double usando el método PutValue
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Guarda el libro de trabajo
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Coloca un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | String | Valor de entrada |
| isConverted | Booleano | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | Booleano | True: establecer el formato numérico al estilo de la celda al convertir a otro tipo de datos |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la celda B3
            Cell cell = worksheet.Cells["B3"];
            
            // Establecer validación de datos para la edad (debe ser un número positivo)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Insertar valor con conversión y verificación de validación
            cell.PutValue("-60", true, false);
            
            // Calcular fórmulas (aunque no es necesario en este caso simple)
            workbook.CalculateFormula();
            
            // Comprobar si el valor es válido
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Guardar el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Coloca un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | String | Valor de entrada |
| isConverted | Booleano | True: convertido a otro tipo de datos si es apropiado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Demostrar PutValue con parámetros string y boolean
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Verificar los valores
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Coloca un valor de cadena en la celda.

```csharp
public void PutValue(string stringValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | String | Valor de entrada |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Usando PutValue con parámetros string
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Guarda el libro de trabajo
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Coloca un valor DateTime en la celda.

```csharp
public void PutValue(DateTime dateTime)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dateTime | DateTime | Valor de entrada |

### Observaciones

Establecer un valor DateTime para una celda no significa que la celda se formatee automáticamente como fecha y hora. El valor DateTime se mantiene como valor numérico en el modelo de datos tanto de MS Excel como de Aspose.Cells. Si el valor numérico se tomará como el propio valor numérico o como fecha y hora depende del formato numérico aplicado a esta celda. Si esta celda no ha sido formateada como fecha y hora, se mostrará como un valor numérico aunque lo que ingresó sea DateTime.

### Ejemplos

Este ejemplo muestra cómo establecer un valor DateTime en una celda y hacer que se muestre como fecha y hora.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Insertar fecha y hora en una celda
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Coloca un valor objeto en la celda.

```csharp
public void PutValue(object objectValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objectValue | Objeto | valor de entrada |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue con objeto DateTime
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue con objeto string
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue con objeto numérico
            cells[2, 0].PutValue((object)123.45);
            
            // Guarda el libro de trabajo
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


