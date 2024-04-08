## Discord register login polosan
source code berguna apa bila kalian ingin membuat website dengan menggunakan sistem login dan di source ini juga sudah mendapatkan auto role dan otomatis join server anda
# konfigurasi
*ikutin configurasi ini yang berada di process-oauth.php
``` $payload = [
  "code"=>$discord_code,
    "client_id"=>"1226068895991988326",#masukin id bot
    "client_secret"=>"uCiXXwSSvlOYIq1RVZe63iuZ2a371nPJ", #masukin secret bot lu
    "grant_type"=>"authorization_code",
    "redirect_uri"=>"http://192.168.1.24:8080/src/process-oauth.php",#masukin ini juga sesuai file ini berada misal lu make lokalhost ya copy aja lokalhost/process-oauth.php
    "scope"=>"identify%20guids",
];```

* apa bila id role ini di isi misal kamu isi admin maka orang yang ada di discord dan memiliki role admin akan di pindahkan ke admin.php sama hal dengan moderator

```$role = "user";
if(in_array("copy id role disini", $guild_roles)){
    $role = "admin";
}else if(in_array("id role ke 2", $guild_roles)){#
    $role = "moderator";
}```

```$guild_ID = "isi dengan guild id";```

```    $botToken = "isi token bot kalian";
    $roleId = "isi role id ini untuk apabila kalian regis maka akan auto ke isi rolenya";```
    
```    $bot_token = "ini juga bot token isi juga";```




# pm discord TheJayඞ#7217 kalo ada yang pusing
