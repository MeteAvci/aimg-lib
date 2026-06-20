# 🔬 SRM Engine

**Scene Reconstruction Manifest – The visual DNA extractor.**

> *"God is dead. God remains dead. And we have killed him. How shall we comfort ourselves, the murderers of all murderers?"*  
> — Friedrich Nietzsche

SRM Engine is a **specialized AI system prompt** that transforms any image into a high-fidelity XML manifest. It doesn't just describe what it sees—it deconstructs the physics, the lighting rig, the PBR materials, and spits out reconstruction blueprints for DALL-E, Flux, Gemini and Imagen.

### Why XML?

JSON is flat. XML is hierarchical. When you're encoding a scene with nested relationships—a `<Vehicle>` containing an `<Engine>` containing `<Pistons>` with their own `<RustLevel>`—you need a structure that mirrors reality. XML's tree structure preserves parent-child relationships, allows inline comments for context, and supports attributes for metadata without polluting the data itself.

### Why This Level of Detail?

Image generators struggle with fine-grained semantics. Vague prompts lead to hallucinations. "A beautiful sunset" gives unpredictable results—but "golden hour, 5500K color temperature, 15° sun angle, volumetric god rays through atmospheric haze" is a precise instruction set. SRM doesn't just describe; it **specifies**. Every surface gets PBR attributes. Every light source gets physics. Every object gets spatial coordinates. The result? Reproducible, cross-platform image generation.

<details>
<summary>🇹🇷 Türkçesi için Tıkla!</summary>

## 🔬 SRM Engine

**Sahne Yeniden Yapım Manifestosu (SRM) – Görsel DNA çıkarıcı.**

> *"Tanrı öldü. Tanrı ölü kalacak. Ve onu biz öldürdük. Katillerin en büyüğü olarak kendimizi nasıl teselli edebiliriz?"*  
> — Friedrich Nietzsche

SRM Engine, herhangi bir görseli yüksek kaliteli XML şablonuna çeviren **özel bir AI sistem komutudur**. Sadece gördüğünü anlatmaz—fiziği, ışık düzenini, yüzey malzemelerini ayrıştırır ve DALL-E, Flux, Gemini ve Imagen için kullanıma hazır şablonlar üretir.

### Neden XML?

JSON düzdür. XML hiyerarşiktir. İç içe ilişkiler barındıran bir sahneyi kodlarken—bir `<Araç>` içinde `<Motor>`, onun içinde `<Pistonlar>` ve onların kendi `<PasSeviyesi>` değerleri—gerçekliği yansıtan bir yapıya ihtiyacın var. XML'ın ağaç yapısı ebeveyn-çocuk ilişkilerini korur, bağlam için satır içi yorumlara izin verir ve veriyi kirletmeden metadata için nitelik kullanmana olanak tanır.

### Neden Bu Kadar Detay?

Görsel üretici modeller ince detaylarda zorlanır. Belirsiz talimatlar beklenmedik sonuçlar doğurur. "Güzel bir gün batımı" tahmin edilemez çıktılar verir—ama "altın saat, 5500K renk sıcaklığı, 15° güneş açısı, atmosferik sisin içinden geçen volumétrik tanrı ışınları" kesin bir talimat setidir. SRM sadece tarif etmez; **tanımlar**. Her yüzeye 3D malzeme özellikleri atanır. Her ışık kaynağına fizik eklenir. Her nesneye uzamsal koordinat verilir. Sonuç? Tekrarlanabilir, platformlar arası görsel üretim.

---

## 🧬 Ne Yapıyor?

| Katman | Ne İş Görüyor |
|--------|---------------|
| **ConceptualCore** | Sahne sınıflandırması, dikkat haritası, stil referansları |
| **TechnicalSpecs** | Kamera ayarları (sensör, lens, diyafram), ışık fiziği |
| **ContentLayer** | Dinamik içerik analizi – konuya göre genişliyor |
| **GenerativeDirectives** | Hazır komutlar: Gemini/Imagen, Midjourney, Flux |

---

## 🎯 Öne Çıkan Özellikler

- **Dinamik Şema** – XML yapısı bir tohum gibi. Model, konuya göre yeni etiketler türetiyor
- **3D Yüzey Standartları** – Renk, pürüzlülük, geçirgenlik, aşınma detayları dahil
- **Sınırsız Detay** – Görselde varsa, XML'de de var
- **Çoklu Platform Çıktısı** – Tek analizden 3 farklı platform için komut

---

## 💻 Nasıl Kullanılır?

SRM Engine'i üç farklı şekilde kullanabilirsin:

### ⚙️ Mod 1: Kalıcı Asistan (Ana Kullanım)

Bu prompt'un asıl yaratılış amacı bu. Bir kere kur, sürekli kullan.

| Platform | Kurulum |
|----------|---------|
| **ChatGPT** | Custom GPT oluştur → Instructions kısmına `srm-engine.md` içeriğini yapıştır |
| **Gemini** | Gem oluştur → Sistem talimatı olarak `srm-engine.md` ekle |
| **Claude** | Projects → Instructions alanına yapıştır |
| **API** | `system_prompt` rolüne prompt içeriğini gönder |

Bir kere kurulunca her sohbet otomatik SRM mantığıyla başlıyor—tekrar yapıştırmana gerek yok.

### 🖼️ Mod 2: Görsel Analiz

Elindeki bir görseli parçalayıp yeniden üretilebilir hale getir.

1. `srm-engine.md` içeriğini AI modeline yapıştır
2. Analiz etmek istediğin görseli yükle
3. Model görselin DNA'sını çıkarır: kamera, yüzeyler, ışık
4. XML şablon + platforma özel komutlar (DALL-E, Flux, Gemini, Imagen) al

> 💡 **Not:** Amaç, girdi görselini **tıpatıp aynı** üretebilecek bir XML şablonu oluşturmaktır. Eğer modifikasyon istiyorsan (farklı ışık, farklı açı, stil değişikliği vs.), bunu görselle birlikte açıkça belirtmelisin.

### 📝 Mod 3: Metin ile Konsept Üretimi

Görsel yok, sadece kafandaki sahneyi anlat.

1. `srm-engine.md` içeriğini AI modeline yapıştır
2. Konseptini en basit haliyle anlat: *"terk edilmiş benzinlik, gün batımı"*
3. Model bu iki kelimeyi alır, fiziğinden ışığına kadar her detayı ekleyerek mükemmel bir XML şablona dönüştürür

---

## 📁 Dosyalar

| Dosya | Açıklama |
|-------|----------|
| `srm-engine.md` | Ana sistem prompt'u |
| `srm-inspire.xml` | Kopyalamadan özgün konsept üreten, tamamen XML Inspire Mode sistem prompt'u |
| `README.md` | Bu dosya |

---

## 👤 Yapımcı

**[Mete Avcı](https://github.com/MeteAvci)** tarafından **AI Final Boss aka ÇeteGPT** ile birlikte yapıldı

[Me the Tech](https://methetech.com) – AI & otomasyon stüdyosu

</details>

---

## 🧬 What It Does

| Layer | Description |
|-------|-------------|
| **ConceptualCore** | Scene classification, visual saliency map, style anchors |
| **TechnicalSpecs** | Optical stack (sensor, lens, aperture), photon physics (lighting, colorimetry) |
| **ContentLayer** | Polymorphic content analysis – expands based on context |
| **GenerativeDirectives** | Ready-to-use prompts: Gemini/Imagen, Midjourney, Flux |

---

## 🎯 Key Features

- **Polymorphic Schema** – XML structure is a seed. Model invents new tags based on context
- **PBR Standards** – Includes albedo, roughness, SSS, wear and imperfection details
- **Infinite Granularity** – If it exists visually, it exists in XML
- **Multi-Model Output** – Single analysis produces 3 platform-specific prompts

---

## 💻 Usage

SRM Engine can be used in three different modes:

### ⚙️ Mode 1: Persistent Assistant (Primary Use)

This is the intended way to use this prompt. Set it once, use it forever.

| Platform | How To |
|----------|--------|
| **ChatGPT** | Create Custom GPT → Paste `srm-engine.md` in Instructions |
| **Gemini** | Create a Gem → Add `srm-engine.md` as System Prompt |
| **Claude** | Projects → Paste in Instructions section |
| **API** | Send prompt content in `system_prompt` role |

Once set up, every conversation automatically starts with SRM Engine logic—no need to paste it each time.

### 🖼️ Mode 2: Image Analysis

Reverse-engineer an existing image into a reproducible manifest.

1. Paste `srm-engine.md` content to an AI model
2. Upload the image you want to analyze
3. Model extracts the visual DNA: optical stack, PBR surfaces, lighting physics
4. Receive XML manifest + platform-specific prompts (DALL-E, Flux, Gemini, Imagen)

> 💡 **Note:** The goal is to create an XML manifest that can reproduce the input image **exactly as-is**. If you want modifications (different lighting, angle, style changes, etc.), specify them explicitly along with the input image.

### 📝 Mode 3: Text-Based Concept Generation

No image needed—just describe the scene in your head.

1. Paste `srm-engine.md` content to an AI model (Gemini, GPT-4, Claude)
2. Describe your concept in plain language: *"abandoned gas station, sunset"*
3. Model takes those two words and transforms them into a perfect XML manifest—adding all the physics, lighting, and material details for you

---

## 📁 Files

| File | Description |
|------|-------------|
| `srm-engine.md` | Main system prompt |
| `srm-inspire.xml` | Fully XML Inspire Mode system prompt for original concepts without reconstruction |
| `README.md` | This file |

---

## 👤 Author

Built by **[Mete Avcı](https://github.com/MeteAvci)** with **AI Final Boss aka ÇeteGPT**

Part of [Me the Tech](https://methetech.com) – AI & automation studio

[![X](https://img.shields.io/badge/@HorizonHacker-000?logo=x)](https://x.com/HorizonHacker)
[![LinkedIn](https://img.shields.io/badge/meteee-0A66C2?logo=linkedin)](https://linkedin.com/in/meteee)

---

## License

[CC0 1.0](../LICENSE)
# SRM Engine

SRM now ships with two complementary modes:

| Mode | Purpose | Prompt |
|---|---|---|
| Reconstruction | Encodes a source image as a high-fidelity XML reconstruction manifest | [srm-engine.md](./srm-engine.md) |
| Inspire | Extracts abstract visual principles and invents a structurally original concept | [srm-inspire.xml](./srm-inspire.xml) |

Use Reconstruction when fidelity is the goal. Use Inspire when the reference should influence the result without being copied.
