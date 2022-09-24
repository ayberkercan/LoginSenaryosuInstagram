# LoginSenaryosuInstagram
instagram login senaryosunu otomatize edeceğim.

Önce otomatize edeceğimiz senaryo’yu adım adım yazalım;
— İnstagram URL’ine gidilir.
— Username girilir.
— Username ile eşleşmeyen parola girilir.
— Log In butonuna basılır.
— Browser, test sonunda kapatılır.

Aşağıda senaryoların kod’a dönüşmüş halini görebilirsiniz ;

— driver.get(loginUrl); //setUp methodunda tanımladığımız loginUrl çağırılır
— driver.findElement(xpath(“//input[@name=’username’]”)).sendKeys
(“testdenemesi”); //username alanına testdenemesi yazılır
— driver.findElement(xpath(“//input[@name=’password’]”)).sendKeys
(“123456”); //password alanına 123456 yazılır
— driver.findElement(xpath(“//div[contains(text(),’Log In’)]”)).click();
//Log In butonuna basılır
— driver.quit(); //Tarayıcıyı kapatılır ve test sonlanır.
