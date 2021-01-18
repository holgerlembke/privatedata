# privatedata

Simple concept to offload all private data you need in your sketches to a central file.

Now you can publish/copy your sketch sources without fear of jeopardizing your data accidentally.

# How to use?

* Download https://github.com/holgerlembke/privatedata/archive/main.zip 
* put into your Lib-Folder
* edit privatedata.h
* use it
* enjoy.

```
#include <privatedata.h>

const char* ssid = privatedata_mySSID;
const char* key = privatedata_myWAP2;

...
  mail->Host = privatedata_SMTPHOST;
...
  mail->Username = privatedata_SMTPUSERNAME;
  mail->Password = privatedata_SMTPPASSWORD;

...
  WiFi.mode(WIFI_STA);
  WiFi.begin(ssid, key);
...
```
