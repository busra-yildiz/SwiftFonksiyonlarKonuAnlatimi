# SwiftFonksiyonlarKonuAnlatimi
Swift programlama dilinde fonksiyonlar, belirli bir işlevi gerçekleştiren bağımsız kod bloklarıdır. Fonksiyonlar, 
kodunuzu düzenlemek, tekrar kullanmak ve daha okunabilir hale getirmek için kullanılır. Swift'te fonksiyonlar hakkında bilmeniz 
gereken temel kavramları aşağıda açıklıyorum:

Fonksiyon Tanımlama
Bir fonksiyon tanımlamak için func anahtar kelimesini kullanırız. Temel bir fonksiyon tanımı şu şekildedir:
func adiFonksiyon() {
    // Fonksiyonun yapılacak işlemleri
}
Örnek bir fonksiyon tanımı:

func selam() {
    print("Merhaba, Dünya!")
}

Parametreler
Fonksiyonlar parametreleri kabul edebilir, böylece farklı değerlerle çalışabilirler. Parametreler fonksiyonun içinde 
kullanılabilir. Örnek bir fonksiyon tanımı:

func toplam(a: Int, b: Int) {
    let sonuc = a + b
    print("Toplam: \(sonuc)")
}

Bu fonksiyon iki tane Int türünde parametre (a ve b) alır ve bunları toplar.

Geri Dönüş Değeri
Bir fonksiyon, işlem sonucunu döndürebilir. Bu, fonksiyonun geri dönüş değeri (return value) olarak adlandırılır. Örnek bir fonksiyon tanımı:

func toplam(a: Int, b: Int) -> Int {
    let sonuc = a + b
    return sonuc
}

Bu fonksiyon iki Int türünde parametre alır ve bu parametreleri toplar, ardından sonucu bir Int olarak geri döndürür.

Fonksiyon Çağırma
Bir fonksiyonu çağırmak için fonksiyon adını ve gerekli parametreleri belirtmelisiniz. Örnek:

selam() // "Merhaba, Dünya!" yazdırır

let sonuc = toplam(a: 5, b: 3)
print(sonuc) // "Toplam: 8" yazdırır

Parametre Etiketleri ve İç Parametre İsimleri
Swift'te fonksiyonlar, hem parametre etiketleri (external parameter labels) hem de iç parametre isimleri
(internal parameter names) kullanabilir. Parametre etiketleri, bir fonksiyon çağırılırken kullanılan adlardır 
ve daha okunabilir çağrılar yapmanıza yardımcı olur. İç parametre isimleri ise fonksiyonun içinde kullanılan adlardır. Örnek:

func toplam(_ a: Int, _ b: Int) -> Int {
    return a + b
}

let sonuc = toplam(5, 3) // Parametre etiketleri kullanılmadan çağırılır


Varsayılan Parametre Değerleri
Fonksiyonlara varsayılan parametre değerleri atanabilir, böylece çağırırken parametre belirtilmezse bu varsayılan değerler kullanılır. Örnek:

func selam(isim: String = "Misafir") {
    print("Merhaba, \(isim)!")
}

selam() // "Merhaba, Misafir!" yazdırır
selam(isim: "Ahmet") // "Merhaba, Ahmet!" yazdırır

İç İşlevler (Nested Functions)
Swift'te, bir fonksiyon başka bir fonksiyon içinde tanımlanabilir. Bu tür fonksiyonlara iç işlevler denir. İç işlevler, dışarıdan erişilemezler ve 
genellikle dış fonksiyonun belirli bir görevi gerçekleştirmesine yardımcı olmak için kullanılır.

İşlev Türleri (Function Types)
Swift, işlevleri bir tür olarak ele alır. Bu, bir fonksiyonun başka bir fonksiyonun parametresi olarak geçebileceği veya bir fonksiyonun 
geri dönüş değeri olarak kullanılabileceği anlamına gelir. İşlev türleri, Swift'in güçlü tür sisteminin bir parçasıdır.

Bu, temel Swift fonksiyonlarının bazı kavramlarıdır. Fonksiyonlar, kodunuzun daha modüler ve düzenli hale gelmesine yardımcı olur ve 
aynı işlemi tekrar tekrar yazmanızı önler. Swift'in güçlü tür sistemi sayesinde, işlevlerle çalışmak daha güvenlidir ve hataları azaltır.
