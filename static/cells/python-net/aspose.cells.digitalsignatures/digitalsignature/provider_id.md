##provider_id property
## provider_id property
Specifies the class ID of the signature provider.
Default value is Empty (all zeroes) Guid.
### Remarks
The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption.
Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider,
and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider.
The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.
### Definition:
```python
@property
def provider_id(self):
...
@provider_id.setter
def provider_id(self, value):
...
```
### See Also
* module [`aspose.cells.digitalsignatures`](../../)
* class [`DigitalSignature`](/cells/python-net/aspose.cells.digitalsignatures/digitalsignature)
