---
title: "Clase ComboBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.ComboBox. Representa un control de lista desplegable de celda"
type: docs
url: /es/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

Representa un control de cuadro combinado de celda.

```csharp
public class ComboBox : CellControl
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Obtiene o establece la altura del control de lista. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Indica si el usuario puede introducir texto en la lista desplegable. El texto introducido se guardará como el valor de la celda. El valor predeterminado es "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Obtiene un objeto que representa la colección de los elementos contenidos en este ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Obtiene o establece el índice que especifica el elemento seleccionado actualmente. Establecer el índice llamará al método GridDesktop.RunAllFormulas automáticamente si la propiedad GridDesktop.RecalculateFormulas es verdadera. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Obtiene o establece el texto asociado a este control.(Heredado de [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Obtiene un objeto que representa la colección de los valores contenidos en este ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Obtiene o establece el ancho del control de lista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Establece el índice seleccionado del ComboBox. Esto no calculará la fórmula. Para calcular la fórmula, es necesario llamar a GridDesktop.RunAllFormulas manualmente. No calculará automáticamente las fórmulas en ningún caso, incluso si GridDesktop.RecalculateFormulas es verdadero. |

### Ver también

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


