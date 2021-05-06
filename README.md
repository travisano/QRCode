# QRPortal
Cisco QR Portal Demo

*Adding A Product to the QR Portal*

1. Create a product profile and add it into qrcode.json configuration file. Note: Include all fields below, feel free to leave blank if irrelevant:

```json
	"c9200l" : {
               "family": "CATALYST C9200L",
               "spec": "https://www.cisco.com/c/en/us/products/collateral/switches/catalyst-9200-series-switches/nb-06-cat9200-ser-data-sheet-cte-en.pdf",
               "pc" :"78-101287-01_A0.pdf",
               "vendor" :"CISCO",
               "doc": "https://www.cisco.com/c/en/us/products/switches/catalyst-9200-series-switches/index.html",
               "extras" : ""
		   }
```

2. Put pointer card ("pc") document into docs/ folder.
