# Kodland Assessment
Öğrenci size hatalı bir proje gönderdi ve bunları düzeltmeniz gerekiyor.
Kodda bir şey eksikse, eklenmesi gerekir.

## Gereksinimler
- Karakteri hareket ettirin
- Kamerayı yönetin
- Fareye sol tıklamak bir mermiyi serbest bırakır
- Uzaylılarla etkileşime girerken, mermi yok edilir ve uzaylılar yok edilir
- Üç düşmanı öldürün

## Görev Gereksinimleri
- Tüm hataları ayrı bir dosyada bulun ve yazın
- Onları düzelt
- Eksik kodu ekle

# Hata Listesi
1. Oyunu başlattığımızda kaybettin ekranı çıkıyor.
2. Player'ın sol tıka bastıgında ateş edememesi -> PlayerController Componentındaki bullet referansının verilmemesi.
3. Player'ın haraket edememesi.
4. Player'ın Kamerayı kontrol edememesi.
5. Bullet'lerin Enemy ile interact olmaması

## Çözümler
### 1. Hatanın Çözümü
Startta ChangeHealth(0) girilmesi sonucu ChangeHealth fonksiyonun Lose fonksiyonunu çağırması önlemek. https://github.com/gamecem/Kodland-Assessment--/commit/561b9b60d4195a924b2731c6ca66e36095d867f4
### 2. Hatanın Çözümü
Ateş etmeye yarayan kodda prefabın player objesinin playercontroller componentine bulletın atanmaması sonucu oluşan hatayı bullet prefabını atayarak çözmek.
### 3. Hatanın Çözümü
Player'ın haraket etme kodunu yazmak. Character Controller kullanarak. https://github.com/gamecem/Kodland-Assessment--/commit/0784eb504fdb35e88dabc3aa731ae64dff365965
### 4. Hatanın Çözümü 
Player'ın PlayerLook componentine inspectorden mouse sense 0 olan değeri arttırarak sorunu çözüyoruz.
### 5. Hatanın Çözümü
Bullet prefabında sadece bullet componentinin bulunması. Collider ve Rigidbodysini verip Enemy'e de Colliderını verip Tagını verdikten sonra kodlarını da güncelleyerek sorunu çözüyoruz. https://github.com/gamecem/Kodland-Assessment--/commit/39b57f9e8155950da1ddd3f6d6fb0864ec610beb
### Ekstra Çözümler
Gereksiz Componentlerin silinmesi. Animatorler, Enemydeki Character Controller vb.

