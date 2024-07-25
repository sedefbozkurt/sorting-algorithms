### Aşamalar

#### 1. Bölme (Divide)

Dizi, mümkün olduğunca küçük parçalara bölünür.

- Başlangıç dizisi: `[16, 21, 11, 8, 12, 22]`
- Orta noktadan bölünür: `[16, 21, 11]` ve `[8, 12, 22]`
- Bu alt diziler de tekrar bölünür: `[16]`, `[21, 11]` ve `[8]`, `[12, 22]`
- Daha da küçük parçalara bölünür: `[21]` ve `[11]` ile `[12]` ve `[22]`

#### 2. Birleştirme (Conquer)

Bu küçük parçalar sıralanmış şekilde birleştirilir.

- `[21]` ve `[11]` birleşir ve sıralanır: `[11, 21]`
- `[12]` ve `[22]` birleşir ve sıralanır: `[12, 22]`
- Küçük sıralı diziler tekrar birleşir: `[16]` ve `[11, 21]` birleşir: `[11, 16, 21]`
- `[8]` ve `[12, 22]` birleşir: `[8, 12, 22]`
- Son olarak, bu iki büyük dizi birleşir: `[11, 16, 21]` ve `[8, 12, 22]`
- Sıralı birleşim sonucu: `[8, 11, 12, 16, 21, 22]`

### Merge Sort Adımları

1. Başlangıç dizisi: `[16, 21, 11, 8, 12, 22]`
2. Bölme: `[16, 21, 11]` ve `[8, 12, 22]`
3. Bölme: `[16]`, `[21, 11]` ve `[8]`, `[12, 22]`
4. Bölme: `[21]`, `[11]` ve `[12]`, `[22]`
5. Birleştirme: `[11, 21]`, `[12, 22]`
6. Birleştirme: `[11, 16, 21]`, `[8, 12, 22]`
7. Birleştirme: `[8, 11, 12, 16, 21, 22]`

### Big-O Gösterimi

Merge Sort algoritmasının zaman karmaşıklığı her zaman `O(n log n)`'dir. Bunun nedeni, her bir bölme işleminin `log n` adımda yapılması ve her birleştirme işleminin `O(n)` adımda yapılmasıdır. Toplamda bu iki işlem, `O(n log n)` zaman karmaşıklığını oluşturur. Merge Sort, en kötü, en iyi ve ortalama durumlarda aynı zaman karmaşıklığına sahiptir: `O(n log n)`.
