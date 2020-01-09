# LittleNet
Flask based IoT Server



### Features

* **Dangerously Simple (Sorry Einstein Ji)**
* Token auth
* Upload Files
* Store Key,Value pair
* Web interface to browse files
* Web interface to view json stored
* Graph for time series data


### Uses

```
import littlenet as ln
ln.init("localhost", port=1200)
```

* Store Data (single)
```
ln.save("key", "value")
```

* Store Data (multiple)
```
ln.store("key", "value")
ln.store("key2", "value2")
ln.commit()
```

* Get Data
```
value= ln.get("key", default= null)
```

* Upload File
```
filepath= "/files/yak.png"
ln.upload("key", filepath)
```

* Download File
```
download_path= "folder"
file= ln.download("key", download_path)
```

* Store JSON
```
ln.savej("key", obj)
```

* Get JSON
```
jobj= ln.getj("key")
```

* Create Record
```
rec= ln.get_record("temperature")  #Create or Get record
rec.add(34)
rec.add(65)
rec.add(565)
rec.add(98)
```
