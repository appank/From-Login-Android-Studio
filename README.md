# From-Login-Android-Studio
From Login biasa tanpa menggunkan Data Base

- <b>MainActivity.java</b> <p>
**Username dan Password yang digunakan**
```MainActivity.java
if (usernameKey.equals("appank") && passwordKey.equals("1")){
```
**Data username di ambil menuju ke <b>activity2</b>**
```MainActivity.java
 String value = username.getText().toString();
                intent.putExtra("yourkey1", value);
                startActivityForResult(intent, REQUEST_CODE);
```
- <b>MainActivity2.java</b> <p>
**Data Username yang di ambil di <b>activity</b>**
```MainActivity.java
 Bundle extras1 = getIntent().getExtras();
        String intent = extras1.getString("yourkey1");
        username = (TextView) findViewById(R.id.username);
        username.setText(intent);
```
 
<i>cek youtube : "<a> https://www.youtube.com/watch?v=4XTwSBzuM2E</a>"</i>   
  
