---
title: "Cell.PutValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Inserisce un valore booleano nella cella"
type: docs
url: /it/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Inserisce un valore booleano nella cella.

```csharp
public void PutValue(bool boolValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| boolValue | Booleano |  |

### Esempi

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

            // Inserisci un valore booleano nella cella B3 (riga 2, colonna 2)
            cells[2, 2].PutValue(true);

            // Verifica che il valore sia stato impostato correttamente
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Inserisce un valore intero nella cella.

```csharp
public void PutValue(int intValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intValue | Int32 | Valore di input |

### Esempi

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
            
            // Utilizzando PutValue con parametri Int32
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Calcola la somma dei valori
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Inserisce un valore double nella cella.

```csharp
public void PutValue(double doubleValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleValue | Double | Valore di input |

### Esempi

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
            
            // Inserisci valori double usando il metodo PutValue
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Salva la cartella di lavoro
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Inserisce un valore nella cella; se appropriato, il valore sarà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | String | Valore di input |
| isConverted | Booleano | True: convertito in un altro tipo di dato se appropriato. |
| setStyle | Booleano | True: imposta il formato numerico nello stile della cella quando si converte in un altro tipo di dato |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la cella B3
            Cell cell = worksheet.Cells["B3"];
            
            // Imposta la convalida dei dati per l'età (deve essere un numero positivo)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Inserisci valore con conversione e verifica della convalida
            cell.PutValue("-60", true, false);
            
            // Calcola le formule (anche se non necessario in questo caso semplice)
            workbook.CalculateFormula();
            
            // Verifica se il valore è valido
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Salva cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dato, se appropriato.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | String | Valore di input |
| isConverted | Booleano | True: convertito in un altro tipo di dato se appropriato. |

### Esempi

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

            // Dimostra PutValue con parametri stringa e booleani
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Verifica i valori
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Inserisce un valore stringa nella cella.

```csharp
public void PutValue(string stringValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | String | Valore di input |

### Esempi

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
            
            // Utilizzo di PutValue con parametri stringa
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Salva la cartella di lavoro
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Inserisce un valore DateTime nella cella.

```csharp
public void PutValue(DateTime dateTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTime | DateTime | Valore di input |

### Osservazioni

Impostare un valore DateTime per una cella non significa che la cella verrà formattata automaticamente come data e ora. Il valore DateTime viene mantenuto come valore numerico nel modello dati sia di MS Excel sia di Aspose.Cells. Se il valore numerico verrà interpretato come valore numerico stesso o come data e ora dipende dal formato numerico applicato a questa cella. Se questa cella non è stata formattata come data e ora, verrà visualizzata come valore numerico anche se l'input è DateTime.

### Esempi

Questo esempio mostra come impostare un valore DateTime in una cella e farlo visualizzare come data e ora.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Inserisci data e ora in una cella
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Inserisce un valore oggetto nella cella.

```csharp
public void PutValue(object objectValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objectValue | Object | valore di input |

### Esempi

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
            
            // PutValue con oggetto DateTime
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue con oggetto stringa
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue con oggetto numerico
            cells[2, 0].PutValue((object)123.45);
            
            // Salva la cartella di lavoro
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


