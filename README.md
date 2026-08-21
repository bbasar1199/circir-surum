# CIRCIR - Surum Duyurusu

Bu depo yalniz **surum bilgisini** tasir; program dosyasi burada durmaz.

CIRCIR / MISIR / YAG kurulumlari acilista `surum.json` dosyasina bakar.
Buradaki surum, calisan programin surumunden yeniyse kullaniciya
"Yeni surum hazir" uyarisi gosterilir ve Hakkinda ekraninda indirme
baglantisi cikar. Dosyaya erisilemezse program tamamen sessiz kalir.

## Yeni surum cikarken

1. `PAKETLE.ps1` calistirilir; `DAGITIMsurum.json` kendiliginden uretilir
   (surum = derleme aninin yil.ay degeri).
2. O dosya bu depodaki `surum.json` uzerine yuklenir (surukle-birak yeter).
3. Kurulum EXE'si Releases bolumune eklenir.

## surum.json alanlari

| Alan | Anlami |
|---|---|
| `surum` | Yeni surum numarasi (`yy.MM`, or. `26.09`) |
| `adres` | Kullanicinin indirmek icin gidecegi adres |
| `not` | Istege bagli kisa aciklama ("kantar duzeltmeleri" gibi) |
