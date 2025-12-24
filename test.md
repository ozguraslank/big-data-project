flowchart TD
    A[Kaynak Veri] --> B[DataFrame Oluşturma]
    B --> C["'-' → null dönüşümü"]
    C --> D[Eksik Oranlarını Hesapla]
    D --> E[Imputation Stratejisi Seç]
    E --> F[Imputer.fit()]
    F --> G[Imputer.transform()]
    G --> H[Doldurulmuş Veri Seti]