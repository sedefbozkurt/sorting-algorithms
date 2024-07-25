# Sorting Algorithms

## Insertion Sort Aşamaları

Verilen dizi: `[22, 27, 16, 2, 18, 6]`

Insertion Sort aşamaları:

1. İlk eleman (22) zaten sıralı kabul edilir.
   - Dizi: `[22, 27, 16, 2, 18, 6]`
2. 27 elemanı yerinde, 22'den büyük olduğu için değiştirmez.
   - Dizi: `[22, 27, 16, 2, 18, 6]`
3. 16 elemanı 27'den küçük olduğu için 27 ile yer değiştirir sonra 22'den de küçük olduğu için onunla da yer değiştirir.
   - Dizi: `[16, 22, 27, 2, 18, 6]`
4. 2 elemanı 27'den küçük olduğu için 27 ile yer değiştirir sonra 22'den küçük olduğu için 22 ile yer değiştirir sonra 16'dan küçük olduğu için 16 ile de yer değiştirir.
   - Dizi: `[2, 16, 22, 27, 18, 6]`
5. 18 elemanı 27'den küçük olduğu için 27 ile yer değiştirir sonra 22'den küçük olduğu için 22 ile yer değiştirir, 16'dan büyük olduğu için 16'nın sağında kalır.
   - Dizi: `[2, 16, 18, 22, 27, 6]`
6. 6 elemanı 27'den küçük olduğu için 27 ile yer değiştirir sonra 22'den küçük olduğu için 22 ile yer değiştirir sonra 18'den küçük olduğu için 18 ile yer değiştirir sonra 16'dan küçük olduğu için 16 ile yer değiştirir, 2'den büyük olduğu için 2'nin sağında kalır.
   - Dizi: `[2, 6, 16, 18, 22, 27]`

### Big-O Gösterimi

Insertion Sort'un Big-O notasyonu:
- En kötü durum (Worst Case): \( O(n^2) \)
- Ortalama durum (Average Case): \( O(n^2) \)
- En iyi durum (Best Case): \( O(n) \)

### Time Complexity: 18 sayısının case durumu

18 sayısı sıralandıktan sonra ortada yer almaktadır bu yüzden Average case kapsamına girer.

## Selection Sort İlk 4 Adım

Verilen dizi: `[7, 3, 5, 8, 2, 9, 4, 15, 6]`

Selection Sort ilk 4 adımı:

1. İlk adım: En küçük eleman olan 2, ilk eleman olan 7 ile yer değiştirir.
   - Dizi: `[2, 3, 5, 8, 7, 9, 4, 15, 6]`
2. İkinci adım: Kalan dizide en küçük eleman 3 zaten ikinci sırada olduğu için yer değiştirmez.
   - Dizi: `[2, 3, 5, 8, 7, 9, 4, 15, 6]`
3. Üçüncü adım: Kalan dizide en küçük eleman olan 4, üçüncü sıradaki 5 ile yer değiştirir.
   - Dizi: `[2, 3, 4, 8, 7, 9, 5, 15, 6]`
4. Dördüncü adım: Kalan dizide en küçük eleman olan 5, dördüncü sıradaki 8 ile yer değiştirir.
   - Dizi: `[2, 3, 4, 5, 7, 9, 8, 15, 6]`
