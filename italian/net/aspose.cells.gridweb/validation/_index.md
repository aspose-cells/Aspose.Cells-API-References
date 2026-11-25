---
title: "Classe Validation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Validation."
type: docs
url: /it/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Validation](validation/#constructor)() | Il costruttore predefinito. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Ottiene la cella relativa dell'oggetto. (Ereditato da [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Ottiene o imposta il nome della funzione JavaScript di convalida client. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Ottiene o imposta il tipo di operazione di validazione, Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Ottiene o imposta il valore target dell'operatore 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Ottiene o imposta il valore target dell'operatore 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Ottiene o imposta se il valore della cella è obbligatorio. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Ottiene o imposta la stringa dell'espressione regolare. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Ottiene l'oggetto lista di valori. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Utilizzato solo in fase di progettazione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Carica l'elenco dei valori da un oggetto DataView. È possibile specificare il campo valore e il campo testo del DataView. Ogni coppia valore e testo verrà combinata in una singola stringa, con una virgola tra di esse. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Si prega di utilizzare GridValidation invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Vedi anche

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


