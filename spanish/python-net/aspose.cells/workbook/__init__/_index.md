---
title: Workbook constructor
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 10
url: /es/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
Inicializa una nueva instancia de la clase [Workbook](/cells/es/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  Observaciones

El tipo de formato de archivo predeterminado es Xlsx. Para crear otro tipo de archivo de formato, utilice Workbook (FileFormatType).
###  Ejemplo


El siguiente código muestra cómo usar el constructor Workbook para crear e inicializar una nueva instancia de la clase.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
Inicializa una nueva instancia de la clase [Workbook](/cells/es/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/es/python-net/aspose.cells/fileformattype) | El nuevo formato de archivo.|
###  Observaciones

El tipo de formato de archivo predeterminado es Excel97To2003.
###  Ejemplo


El siguiente código muestra cómo usar el constructor Workbook para crear e inicializar una nueva instancia de la clase.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
Inicializa una nueva instancia de la clase [Workbook](/cells/es/python-net/aspose.cells/workbook) y abre un archivo.



```python
def __init__(self, file):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| file | str | El nombre del archivo.|


##  Workbook(stream) {#io.RawIOBase}
Inicializa una nueva instancia de la clase [Workbook](/cells/es/python-net/aspose.cells/workbook) y abre una secuencia.



```python
def __init__(self, stream):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| stream | io.RawIOBase | La corriente.|


##  Workbook(file, load_options) {#str-LoadOptions}
Inicializa una nueva instancia de la clase [Workbook](/cells/es/python-net/aspose.cells/workbook) y abre un archivo.



```python
def __init__(self, file, load_options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| file | str | El nombre del archivo.|
| load_options | [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions) | Las opciones de carga|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
Inicializa una nueva instancia de la clase [Workbook](/cells/es/python-net/aspose.cells/workbook) y abre el flujo.



```python
def __init__(self, stream, load_options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| stream | io.RawIOBase | La corriente.|
| load_options | [LoadOptions](/cells/es/python-net/aspose.cells/loadoptions) | Las opciones de carga|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
