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
6. ChangeHealth fonksiyonun int alması ama health değişkenin float verilmesi

## Çözümler
### 1. Hatanın Çözümü
Startta ChangeHealth(0) girilmesi sonucu ChangeHealth fonksiyonun Lose fonksiyonunu çağırması önlemek. https://github.com/gamecem/Kodland-Assessment--/commit/561b9b60d4195a924b2731c6ca66e36095d867f4


