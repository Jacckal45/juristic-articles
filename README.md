# Juristic Blog Content

Bu repository, hukuk blog içeriklerini yönetmek için kullanılmaktadır. Blog içerikleri markdown formatında tutulmakta ve web sitesinde dinamik olarak görüntülenmektedir.

## Repository Yapısı

```
juristic-blog/
├── articles/           # Markdown formatında blog yazıları
├── images/            # Blog görselleri
├── metadata.json      # Blog yazılarının meta verileri
└── README.md         # Bu dosya
```

## Yeni Blog Yazısı Ekleme

1. `articles/` klasörüne yeni bir markdown dosyası ekleyin (örn: `yeni-makale.md`)
2. `metadata.json` dosyasına yeni makalenin meta verilerini ekleyin:

```json
{
  "id": "9",
  "title": "Makale Başlığı",
  "slug": "makale-slug",
  "image": "images/makale-resmi.jpg",
  "thumb": "Avukat, Hukuk",
  "description": "Makale açıklaması",
  "author": "Yazar Adı",
  "authorTitle": "Unvan",
  "create_at": "Tarih",
  "comment": "0",
  "blClass": "format-standard-image"
}
```

3. Makale görselini `images/` klasörüne ekleyin

## Markdown Formatı

Blog yazılarınızı markdown formatında yazarken şu yapıyı kullanın:

```markdown
# Makale Başlığı

Giriş paragrafı...

## Alt Başlık 1

İçerik...

## Alt Başlık 2

İçerik...

## Sonuç

Sonuç paragrafı...
```

## Görseller

- Görseller `images/` klasöründe saklanır
- Görsel isimleri küçük harflerle, türkçe karakter içermeyecek şekilde olmalıdır
- Desteklenen formatlar: .jpg, .png, .webp
- Önerilen görsel boyutları: 800x600px

## Deployment

Bu repository'deki içerikler web sitesinde otomatik olarak görüntülenir. Yeni bir içerik eklediğinizde veya mevcut içeriği güncellediğinizde, değişiklikler web sitesine otomatik olarak yansıyacaktır.
