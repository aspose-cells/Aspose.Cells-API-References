##signature_line_type property
## signature_line_type property
Gets or sets the signature type.
Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}.
Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}.
Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider.
### Definition:
```python
@property
def signature_line_type(self):
...
@signature_line_type.setter
def signature_line_type(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`SignatureLine`](/cells/python-net/aspose.cells.drawing/signatureline)
* class [`SignatureType`](/cells/python-net/aspose.cells.drawing/signaturetype)
