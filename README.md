# QRPortal
Cisco QR Portal Demo

*Adding A Product to the QR Portal*

1. Add your PID keywords to BU_or_PID_families mapping in  qrcode.json configuration file,
   This will map your BU or PID families to a "product profile" ->  Product profile will contain links and pointer card destinations

```
json
    "BU_or_PID_families": {
            "UABU": ["C9200*", "C9300*", "C9400*"],
            "IR1100" : ["IR1101-K9*"]
            },

```
  
2. Create a product profile and add it into qrcode.json configuration file. Note: Include all fields below, feel free to leave blank if irrelevant:

```json
	"IR1100" : {
                 "pc" : "78-101332-02_A0.pdf",
                 "doc" : "https://www.cisco.com/c/en/us/products/collateral/routers/1101-industrial-integrated-services-router/datasheet-c78-741709.html",
                 "extra_buttons" : "<button class=\"button button3\"><b>DNA Center Application<br></b></button>"
		   },
```

2. Put associated pointer card ("pc") document into portal's docs/ folder.

```
docs/78-101287-01_A0.pdf
```

3. (OPTIONAL) For any product-specific addons or specialties, feel free to add contents into "extras" field into your product profile in the form of HTML.  

```json
 "extra_buttons" : "<button class=\"button button3\"><b>DNA Center Application<br></b></button>"
```
