## Thumbnail
![GitHub Logo](/thumbnail.png)
Format: ![Alt Text](url)

## Input otomatis huruf kecil (auto lowercase)
Edit file login.html 
```
// set password = username
function setpass(){
  var user = username.value		
  password.value = user;
}

username.onkeyup = setpass;

```
menjadi
```
// set password = username
function setpass(){
  var user = username.value	
  user = user.toLowerCase();
  username.value = user;	
  password.value = user;
}

username.onkeyup = setpass; 

```
