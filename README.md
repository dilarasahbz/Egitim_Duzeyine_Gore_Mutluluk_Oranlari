# Eğitim Düzeyinde Mutluluk

Uygulamalı İstatistik dersi kapsamında, TÜİK verileri kullanılarak hazırlanan bir istatistik projesidir. Projede eğitim düzeyi ile mutluluk oranı arasındaki ilişki betimsel istatistikler, grafikler, hipotez testleri, ki-kare testleri, F dağılımı ve regresyon analizi ile incelenmiştir.

**Ekip:** 5 kişi

## İçerik

| Dosya | Açıklama |
|---|---|
| `Egitim_Duzeyinde_Mutluluk_Raporu.pdf` | Projenin tam raporu |
| `projeson.qmd` | Analizin yapıldığı R / Quarto kaynak dosyası |
| `projeson.xlsx` | Kullanılan veri seti |
| `eğitim düzeyinde mutluluk oranları.pptx` | Proje sunumu |

## Kullanılan Veri

Veri seti, TÜİK'in hanehalkı araştırmalarından alınan "Eğitim Düzeylerine Göre Mutluluk Oranları" verisidir; 2004-2022 yılları arasını, yükseköğretim, lise ve dengi okul, ilkokul veya ortaokul, ilkokul ve bir okul bitirmedi eğitim düzeylerini kapsar.

## Analiz Adımları

1. Verinin okutulması ve incelenmesi (`readxl`, `str()`, `flextable()`)
2. Betimsel istatistikler (ortalama, medyan, standart sapma, quantile)
3. Grafikler (nokta, histogram, kutu, sütun, daire dilimi, sütun-çizgi)
4. Hipotez testleri (t testi, tek ve iki anakütle oran testi)
5. Ki-kare testleri (bağımsızlık testleri)
6. F dağılımı ve varyans testi
7. Regresyon analizi

## Gereken R Paketleri

```
readxl, tidyverse, knitr, kableExtra, flextable, ggplot2, dplyr, car, ggpubr
```

## Nasıl Çalıştırılır

`projeson.qmd` dosyasını RStudio'da (veya Quarto destekleyen bir ortamda) açıp render edin. `projeson.xlsx` veri dosyasının `.qmd` ile aynı klasörde olması gerekir.

## Sonuç

T testinde 2004 ve 2022 yılları arasında yükseköğretim mezunlarının mutluluk ortalamasında anlamlı bir fark bulunamamıştır; ancak ki-kare bağımsızlık testlerinde hem eğitim düzeyi hem de yıl ile mutluluk arasında istatistiksel olarak anlamlı ilişkiler tespit edilmiştir. Regresyon modelinde eğitim seviyesinin mutluluk üzerinde genel olarak anlamlı bir etkisi olduğu, bu etkinin özellikle yükseköğretim ve ilkokul düzeylerinde belirgin olduğu gösterilmiştir.
