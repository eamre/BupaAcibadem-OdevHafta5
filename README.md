# week5-assignment1

**NORTHWND veri tabanında bulunan tabloların mimariye eklenip, kullanıma hazır duruma getirilmesi**

- a-interface 
- b-bll 
- c-dal 
- d-conroller yapıları 
- e-depency injection yapısına dahil edilmesi 
 
*Bu yapıları mimarimize uygun olacak şekilde implemente edilmelidir.*

*Bu yapıda eğer kullanıcı token almadıysa hiç bir işlem yapmayacak şekilde olmalı*

# week5-assignment2

*Bu sisteme kullanıcının kendisinin kayıt olduğunu düşünerek;*

- Kullanıcı kayıt işlemlerini gerçekleştiren metod(ları) yazınız. 

- Kullanıcı kayıt işlemlerini; kullanıcı kayıt sırasında girdiği paralanın veri tabanına şifreli olarak kayıt olacak şekilde tasarlayınız.


*MD5,SHA1,MD5 (SHA1),SHA1 (MD5)  algoritmalarını tercih edebilirsiniz.*


**Örnek c# MD5 şifreleme metodu**

```
public string MD5Hash(string input) 
{ 
    using (var md5 = MD5.Create()) 
    { 
        var result = md5.ComputeHash(Encoding.ASCII.GetBytes(input)); 
        var strResult = BitConverter.ToString(result); 
        return strResult.Replace("-", ""); 
    } 
}
```
