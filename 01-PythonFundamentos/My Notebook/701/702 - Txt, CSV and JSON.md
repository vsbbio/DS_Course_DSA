## How to handle with TXT, CSV and JSON files

## CSV files
### To Write

    1. with open("filename.csv", "w") as filename
    2. import csv (module)
    3. obj = csv.writer(filename)
    4. obj.writerrow(content)
    
### To read

    1. obj = csv.reader(filename)

## JSON files
### To Write

    1. with open("dados.json", "w") as jsonname !!!encoding="utf8"
    2. import json (module)
    3. json.dumps(dictname) " it convert dictionaries to json"
    4. jsonname.writer(json.dumps(dictname))
    
## Methods
### 1

with open(arquivo_fonte,'r') as infile:
    text = infile.read()
    with open(arquivo_destino,'w') as outfile:
        outfile.write(text) 

### Método 2

open(arquivo_destino,'w').write(open(arquivo_fonte,'r').read()) 
