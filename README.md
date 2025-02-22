# binarysearchtree
Swift eğitimimin bir parçası olan Algoritma ve Veri Yapıları Binary Search Tree konusu icin bir örnek çözüm.



Verilen dizi: **[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]**

### **Adım Adım Binary Search Tree Aşamaları:**

1. **İlk elemanı (7) kök (root) olarak alalım:**
    - Kök (root) = **7**
2. **5'i ekleyelim:**
    - 5, 7'den küçük olduğu için **7'nin soluna** gelir.
    - **Sol alt ağaç:** [5]
3. **1'i ekleyelim:**
    - 1, 7'den küçük, 5'ten de küçük olduğu için **5'in soluna** gelir.
    - **Sol alt ağaç:** [5 -> 1]
4. **8'i ekleyelim:**
    - 8, 7'den büyük olduğu için **7'nin sağına** gelir.
    - **Sağ alt ağaç:** [8]
5. **3'ü ekleyelim:**
    - 3, 7'den küçük, 5'ten küçük, 1'den büyük olduğu için **1'in sağına** gelir.
    - **Sol alt ağaç:** [5 -> 1 -> 3]
6. **6'yı ekleyelim:**
    - 6, 7'den küçük, 5'ten büyük olduğu için **5'in sağına** gelir.
    - **Sol alt ağaç:** [5 -> 1 -> 3, 5 -> 6]
7. **0'ı ekleyelim:**
    - 0, 7'den küçük, 5'ten küçük, 1'den küçük olduğu için **1'in soluna** gelir.
    - **Sol alt ağaç:** [5 -> 1 -> 0, 5 -> 1 -> 3]
8. **9'u ekleyelim:**
    - 9, 7'den büyük, 8'den de büyük olduğu için **8'in sağına** gelir.
    - **Sağ alt ağaç:** [8 -> 9]
9. **4'ü ekleyelim:**
    - 4, 7'den küçük, 5'ten büyük, 1'den küçük, 3'ten büyük olduğu için **3'ün sağına** gelir.
    - **Sol alt ağaç:** [5 -> 1 -> 3 -> 4]
10. **2'yi ekleyelim:**
    - 2, 7'den küçük, 5'ten küçük, 1'den büyük, 3'ten küçük olduğu için **3'ün soluna** gelir.
    - **Sol alt ağaç:** [5 -> 1 -> 3 -> 2, 5 -> 1 -> 3 -> 4]

---

### **Binary Search Tree Sonucu:**

```
markdown
KopyalaDüzenle
              7
            /   \
          5      8
         / \       \
        1   6       9
       / \
      0   3
         /  \
        2    4

```

### **Özet:**

- **Kök (root)**: 7
- **Sol alt ağaç**: 5, 1, 3, 0, 6, 2, 4
- **Sağ alt ağaç**: 8, 9

Diziyi ikili arama ağacına dönüştürme işlemi sırasında, her yeni eleman, uygun konumda ve ağacın sağ ve sol alt ağaç yapısını koruyarak yerleştirilmiştir.
