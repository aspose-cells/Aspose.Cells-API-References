---
title: set_header método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 200
url: /es/python-net/aspose.cells/pagesetup/set_header/
is_root: false
---
##  set_header(section, header_script) {#int-str}
Establece un script que formatea el encabezado de un archivo de Excel.



```python
def set_header(self, section, header_script):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha.|
| header_script | str | Script de formato de encabezado.|
###  Observaciones

Comandos de guión:

| Dominio| Descripción|
| :- | :- |
| &PAG| Número de página actual|
| &NORTE| Recuento de páginas|
| &D| Fecha actual|
| &T| Tiempo actual|
| &A| Nombre de la hoja|
| &F| Nombre de archivo sin ruta|
| &"<FontName>"| Nombre de fuente, por ejemplo: &"Arial"|
| &"<FontName>, <FontStyle>"| Nombre de fuente y estilo de fuente, por ejemplo: &"Arial,Negrita"|
| &<FontSize>| Tamaño de la fuente: si este comando va seguido de un número simple para imprimir en el encabezado, se separará de la altura de la fuente con un carácter de espacio.|
| &K<RRGGBB>|Color de fuente, por ejemplo (ROJO): &KFF0000|
| &GRAMO| Guión de imagen|

Por ejemplo: "&Arial,Negrita&8Nota de encabezado"


###  Ver también
* módulo [aspose.cells](../../)
* clase [PageSetup](/cells/es/python-net/aspose.cells/pagesetup)
