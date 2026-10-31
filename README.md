# PayFlow SQL Analysis

## Project Objective

Bu çalışmanın amacı, PayFlow ödeme işlemleri verisini temel SQL sorguları kullanarak analiz etmektir.

## Dataset

Veri setindeki her satır bir ödeme işlemini temsil etmektedir.

Kullanılan temel alanlar:

- transaction_id
- transaction_date
- customer_segment
- city
- payment_method
- merchant_category
- transaction_amount
- transaction_status
- failure_reason
- device_type
- transaction_hour

## Analysis Scope

Bu projede:

- İşlem sayıları
- İşlem hacimleri
- Ortalama işlem tutarları
- Ödeme yöntemleri
- Müşteri segmentleri
- Şehirler
- Başarısızlık nedenleri

incelenmiştir.

## Key Findings

1. **Ödeme Yöntemi Liderliği:** Credit Card hem işlem adedi hem de hacim bazında açık ara liderdir.
2. **Sektörel Ciro Etkisi:** Travel ve Electronics kategorileri, düşük işlem adetlerine rağmen yüksek sepet tutarlarıyla toplam hacmi sırtlamaktadır.
3. **Başarısızlık Dinamiği:** Başarısız işlemlerin en büyük sebebi yetersiz bakiyedir (`Insufficient Funds`).