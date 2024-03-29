---
title: UpdateSelectedValue
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Aggiorna il valore selezionato in base al valore della cella collegata.
type: docs
weight: 1170
url: /it/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Aggiorna il valore selezionato in base al valore della cella collegata.

```csharp
public void UpdateSelectedValue()
```

### Esempi

```csharp

[C#]
//Inizializza una nuova cartella di lavoro.
//Cartella di lavoro = nuova cartella di lavoro();

Cell cell = null;
for (int i = 0; i< 10; ++i)
{
    cell = book.Worksheets[0].Cells[i, 0];
    cell.Value = i + 1;
}
   
//Crea un oggetto ListBox

//Controlli ActiveX
//Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);

//Controlli modulo
Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddListBox(2, 0, 2, 0, 130, 130);

//Imposta l'intervallo utilizzato per riempire il controllo.
listBox.SetInputRange("$A$1:$A$6", false, false);

//Imposta l'intervallo collegato al valore del controllo.
listBox.SetLinkedCell("$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Imposta il valore della cella A12
cell = book.Worksheets[0].Cells[11, 0];
cell.Value = 3;

//Aggiorna il valore selezionato in base al valore della cella collegata.
listBox.UpdateSelectedValue();

//-1 predefinito, nessuna opzione selezionata
if(listbx.IsSelected(2))
{
    //L'opzione 3 di ListBox è selezionata
}

//Modifica il valore di una cella collegata
cell.Value = 4;

//Aggiorna il valore selezionato in base al valore della cella collegata.
listBox.UpdateSelectedValue();
if(listbx.IsSelected(3))
{
    //L'opzione 4 di ListBox è selezionata
}

```

### Guarda anche

* class [Shape](../../shape)
* spazio dei nomi [Aspose.Cells.Drawing](../../shape)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
