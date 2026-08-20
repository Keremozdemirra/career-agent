---
name: "basvuru-takip"
description: "İş ve staj başvurularını tek dosyada takip eder — yeni başvuru ekler, durumları günceller, hangisine ne zaman dönüş yapılması gerektiğini söyler. \"Başvuru ekle\", \"başvurularım ne durumda\", \"şu şirkete başvurdum\", \"kimden dönüş bekliyorum\", \"takip maili atmalı mıyım\" dendiğinde kullan."
---

# Başvuru Takibi

Tek kaynak: `kariyer/basvurular.md`. Yoksa oluştur.

## Tablo formatı
```
| Şirket | Pozisyon | Kanal | Başvuru | Durum | Son temas | Sonraki adım | Not |
```
**Durum** şunlardan biri: `gonderildi` · `okundu` · `gorusme` · `teklif` ·
`red` · `sessiz` · `vazgectim`

Her satırın altına ilan linkini ve varsa iletişim kişisini yaz.

## Yeni başvuru eklerken
İlan linki verilirse **oku**: pozisyon, şirket, son başvuru tarihi, aranan
nitelikleri çıkar. Kullanıcıya sorma, ilandan al. Ulaşamıyorsan söyle.

Satırı ekle, `Sonraki adım` sütununa **tarih koy** — takip maili için
7 iş günü sonrası varsayılan.

## "Durum ne" dendiğinde
Ham tabloyu dökme. Şunu üret:

```
## Aksiyon bekleyen (N)
- Şirket — Pozisyon — ne yapmalı — kaç gündür bekliyor

## Hareket var
- (son 7 günde durumu değişenler)

## Sessiz  (14+ gün dönüş yok)
- Şirket — takip maili atılsın mı?

## Özet
X aktif · Y görüşme · Z sonuçlandı
```

## Takip maili
`sessiz` durumundakiler için taslak yaz:
- 4-6 cümle, tek soru
- İlgini yeniden göster ama yalvarma tonu yok
- Somut bir şey ekle: yeni bir proje, ilgili bir gelişme
- **Gönderme, taslak göster.**

## Kurallar
- Tarihleri `YYYY-MM-DD` yaz. "geçen hafta" değil.
- Red gelenleri silme, `red` işaretle — hangi tür pozisyonda ne olduğunu
  görmek zamanla desen çıkarır.
- 3+ red aynı aşamada geldiyse (örn. hep teknik mülakatta) bunu söyle;
  desen tesadüf değildir.
- Türkçe yaz.
