# Yapay zekâ karakter şablonu: Kem Göz / Forn

Yapay zekâyla video üretirken karakterinizin her sahnede aynı kalması için kullandığım şablon ve referans görseller.
[Forn AI](https://www.youtube.com/channel/UCRBbZXl8gfgCDS2IDoOK_cQ) kanalındaki "Kem Göz" kısa filminde bu yöntemle çalıştım.

🎬 Filmi yaptığım platform: **Higgsfield** → https://higgsfield.ai/s/higgsfield-general-campaign-yt-fornyapayzeka-HwKIHf

## Nasıl kullanılır?

1. **Karakter sayfası hazırlayın.** Önden, 3/4, yandan, arkadan ve birkaç yüz ifadesiyle. Örnek: [`referans/forn-karakter-sayfasi.png`](referans/forn-karakter-sayfasi.png)
2. **Açıları ayrı görsellere bölün** ve her üretimde referans olarak verin. Örnek: [`referans/`](referans/) klasörü.
3. **Karakter tarifi paragrafını doldurun** ([`sablon.txt`](sablon.txt)) ve **her prompt'un başına aynen koyun.**
   Karakterin en kolay bozulan ayrıntılarını açıkça yazın: göz sayısı, burun, kol/bacak sayısı, el rengi…
4. **Higgsfield'da Element olarak kaydedebilirsiniz**; videolarda karakteri ismiyle çağırırsınız.

## Kredi sırası

Önce plan → sonra görsel → sonra düşük kalitede video → en son büyütme.

| Adım | Higgsfield | Kredi (çekim günü, 22 Ekim 2026) |
|---|---|---|
| Kare | Nano Banana Pro, 4 görsel 1K | 8 (görsel başı 2) |
| Taslak video | Seedance 2.5, 14 sn, 480p | 42 |
| Doğrudan yüksek kalite | Seedance 2.5, 14 sn, 1080p | 224 |
| Büyütme | Edit Video → Upscale, 1080p | ~25 |

Fiyatlar değişebilir; Generate düğmesindeki güncel sayıya bakın.

## Şablon

```
[Name] is the single original [color] [shape] character shown in the reference images. Preserve the exact reference proportions, colors, material and outlines. [Head and body]. [Distinctive detail]. His face has exactly [number] eye(s): [eye details]; [eyebrow], [nose], [mouth]. He has exactly [number] arms and [number] legs: [arms / hands / legs / feet]. Keep the same anatomy, material and proportions in every pose, camera angle and lighting. His default expression is [personality].
```

## Doldurulmuş örnek: Forn

```
Forn is the single original blue, one-eyed disk-shaped cartoon character shown in the reference images. Preserve the exact reference proportions and disk thickness. Deep saturated cobalt blue with dense halftone dot shading that darkens toward the rim, a bright glossy white highlight at the upper left, thick black comic outlines. His head and torso are one continuous circular disk, with a small open hole passing through the disk near its top edge, with a dark inner rim showing the disk's thickness; the hole is separate from his eye. His front face has exactly one large eye: white with a warm cream tint under the heavy blue upper eyelid, bright cyan-blue iris, black pupil with a small white catchlight; one thick black eyebrow stroke, a flat black L-shaped nose mark and a short black mouth line. The back is blank blue apart from the upper hole. He has exactly two blue rubber-hose arms and two blue rubber-hose legs, blue ungloved hands and broad rounded blue feet. Keep the same anatomy, material and proportions in every pose, angle and lighting. His default expression is dry, knowing and mildly unimpressed.
```

## Filmde kullandığım iki gerçek prompt

**Kare (Nano Banana Pro, referans: 3 açı görseli)**: yukarıdaki Forn paragrafı + şu sahne:

```
Scene: an upstairs hallway lit only by a small warm nightlight. Above a child's bedroom door, Forn hangs by a thin red string threaded through the hole at the top of his disk, like a protective charm. His eye is fully closed. Medium shot, door centered, Forn in the upper third.

Style: the glossy illustrated cartoon character with black outlines placed in a cinematic, warm, slightly stylized realistic family home. Low-key night lighting, soft volumetric haze, shallow depth of field, subtle film grain. No text, no letters, no logos anywhere. 16:9.
```

**Video (Seedance 2.5, 14 sn, 480p; tek üretimde 3 çekim)**:

```
Image 1 is the starting frame. Image 2 is the composition for Shot 2. The Forn element is the character identity.

Forn is the single original blue, one-eyed disk-shaped cartoon character from the references. Keep exactly one eye, the small hole near the top edge of his disk, the flat black L-shaped nose, deep cobalt blue glossy surface with halftone shading and thick black outlines.

Shot 1 (0-4s): Wide exterior of the quiet family house at night under the moon; bare branches sway gently. Slow push in toward the warm upstairs window.
Shot 2 (4-9s): Cut to the upstairs hallway lit by a small warm nightlight. Forn hangs by a thin red string above the child's bedroom door, eye closed, perfectly still. Slow dolly in.
Shot 3 (9-14s): Close-up on Forn. His single eye slowly opens; the heavy eyelid stays half-closed, dry and unimpressed. Camera holds still.

Style: cinematic, warm, slightly stylized realistic home, low-key night lighting, soft haze, shallow depth of field, subtle film grain.
Sound: soft wind outside, a clock ticking in the hallway. No music, no dialogue, no subtitles, no text.
```

## Lisans

Şablon ve prompt metinleri serbestçe kullanılabilir. Forn karakteri ve görselleri Forn AI kanalına aittir; kendi karakteriniz için örnek olarak bakın.
