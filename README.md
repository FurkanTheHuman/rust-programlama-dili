# Rust Programlama dili

Bu depo "[The Rust Programming Language]" adlı kitabın Türkçe çevirisini barındırmaktadır.

[The Rust Programming Language]:https://doc.rust-lang.org/stable/book/


## Gereksinimler

Bu kitabın derleme işlemi için [mdBook] paketi gereklidir. En iyi biçimde derleyebilmek için [bu dosya][rust-mdbook]da belirttiğimiz sürümü kullanmalısınız. [mdBook] paketini edinmek için:

[mdBook]: https://github.com/rust-lang-nursery/mdBook
[rust-mdbook]: https://github.com/rust-lang/rust/blob/master/src/tools/rustbook/Cargo.toml

```bash
$ cargo install mdbook --vers [sürüm-numarası]
```

## Derleme

Bu kitabı derlemek için:

```bash
$ mdbook build
```
Çıktı `book` alt dizininde olacaktır. Kontrol etmek için tarayıcınızda açın.

_Firefox:_
```bash
$ firefox book/index.html                       # Linux
$ open -a "Firefox" book/index.html             # OS X
$ Start-Process "firefox.exe" .\book\index.html # Windows (PowerShell)
$ start firefox.exe .\book\index.html           # Windows (Cmd)
```

_Chrome:_
```bash
$ google-chrome book/index.html                 # Linux
$ open -a "Google Chrome" book/index.html       # OS X
$ Start-Process "chrome.exe" .\book\index.html  # Windows (PowerShell)
$ start chrome.exe .\book\index.html            # Windows (Cmd)
```

Test Etmek için:

```bash
$ mdbook test
```

## Katkıda bulunmak

Yardım etmeniz bizi çok mutlu eder. Ne tür katkılar beklediğimizi öğrenmek için lütfen [CONTRIBUTING.md][contrib] dosyasını inceleyin. 

[contrib]: https://github.com/over1ove/rust-programlama-dili/blob/master/CONTRIBUTING.md


## Diyagramlar

Bu kitaptaki bazı diyagramlar için [Graphviz](http://graphviz.org/) kullanıyoruz. Diyagram dosyaları `dot`alt dizini içinde bulunur.
Örnek olarak `dot/trpl04-01.dot` dosyasını .svg ye çevirmek için:

```bash
$ dot dot/trpl04-01.dot -Tsvg > src/img/trpl04-01.svg
```

Oluşturulan SVG dosyasında `width` ve `height` niteliklerini silip `viewBox` niteliğini `0.00 0.00 1000.00 1000.00` olarak değiştirmelisiniz.


## Yazım denetimi

Dosyalardaki yazım hatalarını taramak için `spellcheck.sh` adlı betiği kullanabilirsiniz. Betik, `dictionary.txt` sözlük dosyasına ihtiyaç duymaktadır. Eğer sahte pozitif sonuçlar üretiyorsa ( Örneğin `BTreeMap` kelimesini kullandınız ve tararken hata verdi ) Bu durumda kelimeyi `dictionary.txt` dosyasına eklemelisiniz. ( Tutarlılık için lütfen alfabetik sıralamayı koruyunuz. )
