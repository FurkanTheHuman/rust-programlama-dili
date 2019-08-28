# Stil Rehberi

## Düzyazı

* Bölüm başlıklarını kurallara uygun yaz, Örnek: `Gizli bir numara üretmek` yerine `Gizli Bir Numara Üretmek`.

* Bir terimden bahsederken tek tırnak yerine italik yazı tipi tercih et. Örnek : 'İlişkili fonksiyon' yerine *ilişkili fonksiyon*

* Düzyazı içerisinde bir metoddan bahsederken parantezleri KULLANMA. Örnek: `read_line()` yerine `read_line`.

* Kod ve düzyazıyı tek kelimede kullanma. Örnek: ``Remember when we `use`d `std::io`?`` yerine ``Remember when we wrote
  `use std::io`?``


## KOD

* Kod bloklarında hangi dosyayı kastettiğini anlayabilmemiz için önce dosya adını ekle.

* Kodda değişiklik yaparken anlaşılır olması için; hangi parçanın aynı kaldığını, hangi parçanın değiştirildiğini belirtin.
  
* Uzun satırları 80 karakterden kısa tutmanız iyi olur.

* Komut satırına yazılacak bir şey belirtirken başında `bash` söz dizimi kullanın.

## Linkler

Tüm betikler bittiğinde:

* Eğer bir link ekrana basılmamalıysa, onu yoksayılacak olarak işaretleyin.
  * Bu tüm "Chapter XX" kitap-içi ve HTML sürümü için olan linkleri kapsar. 

* Kitap-içi linkleri ve stdlib API döküman linkleri relative dir. Bu yüzden hem offline hem de docs.rust-lang.org üzerinde çalışırlar. 

* Linkler için markdown kullanın ve onların okunabilir formatta olmasına özen gösterin.
