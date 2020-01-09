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
```

* Store Data
```
ln.store("key", "value")
ln.store("key2", "value2")
ln.commit()
```

* Get Data
```
value= ln.get("key")
```

* Upload File
```
filepath= "/files/yak.png"
ln.upload("key", filepath)
```

* Download File
```
file= ln.download("key")
```
