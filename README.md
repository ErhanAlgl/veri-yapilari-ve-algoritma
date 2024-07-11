## PROJE 1

[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

1. Average case: Aradığımız sayının ortada olması
2. Worst case: Aradığımız sayının sonda olması
3. Best case: Aradığımız sayının dizinin en başında olması.

[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

----------------------------------------------------------------

### Insertion Sort'a göre aşamaları
```
Her öğeyi solundaki öğeler ile karşılaştırarak sıralama yapacağız.
1.Adım: [22,27,16,2,18,6] = Sıralanmış ilk dizi (22) ile başlıyoruz. İlk eleman sıralı olarak kabul edildiği için bir değişiklik olmuyor.
2.Adım: [22,27,16,2,18,6] = (27) ile (22) karşılaştırılıyor. 27 büyük olduğu için yine bir değişiklik olmuyor
3.Adım: [16,22,27,2,18,6] = (16) ile (27) ve (22) karşılaştırılıyor ve (16) en başa geçiyor.
4.Adım: [2,16,22,27,18,6] = (2) ile solundaki sayılar karşılaştırılarak (2) en başa geçiyor.
5.Adım: [2,16,18,22,27,6] = (18) ile solundaki sayılar karşılaştırılarak (18) 3. dizideki yerini alıyor.
6.Adım: [2,6,16,18,22,27] = (6) ile solundaki sayılar karşılaştırılarak doğru yere yerleştiriliyor.

** Sonuç olarak 6 adımda Insertion short'a göre sıralı diziye ulaşmış oluyoruz => [2,6,16,18,22,27]
```
----------------------------------------------------------------

### Big-O gösterimi
```
** O(n2).
```
----------------------------------------------------------------

### Time Complexity
```
** Average case: 18, sıralı dizinin tam ortasında yer almaz ama ortalara yakın bir yerde olduğundan dolayı average case'e daha yakın olarak değerlendirilebilir.
```
----------------------------------------------------------------

### [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımı
```
1.Adım: [2,3,5,8,7,9,4,15,6] = Sayı öbeğinin en küçüğünü bulup en başa alıp en baştaki ile yer değiştirilir. (2) ile (7) yer değiştirdi.
2.Adım: [2,3,5,8,7,9,4,15,6] = 2. elaman (3) numarasından sonra sağ taraftaki dizide en küçük olmadığı için aynı kalacak
3.Adım: [2,3,4,8,7,9,5,15,6] = 3. elaman (5) ile (4) yer değiştirerek. 3.eleman artık (4) olacak.
4.Adım: [2,3,4,5,7,9,8,15,6] = 4. elaman (8) ile (5) yer değiştirerek. 4.eleman artık (5) olacak.

** İlk 4 adım sonucu => [2,3,4,5,7,9,8,15,6]
```
----------------------------------------------------------------

## PROJE 2

[16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.

----------------------------------------------------------------

### Merge Short
```
[16,21,11,8,12,22]
1.Adım    [16,21,11]           [8,12,22]
2.Adım   [16] [21,11]         [8,12] [22]
3.Adım  [16] [21] [11]       [8] [12] [22]
4.Adım   [16] [11,21]         [8,12] [22]
5.Adım    [11,16,21]           [8,12,22]
6.Adım          [8,11,12,16,21,22]
          
** Merge Short türüne göre sonuç => [8,11,12,16,21,22]
```
----------------------------------------------------------------

### Big-O gösterimini
```
** O(nlogn)
```
----------------------------------------------------------------

## PROJE 3

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

----------------------------------------------------------------

### Binary-Search-Tree

*Not: Sağ tarafından kendinden büyük elemanlar, sol tarafında ise kendinden küçük elemanlar bulunacak.*
*Not: Root genellikle ilk eleman seçilir.*

Adımlar;
```
1.Adım: Root 7'dir.
2.Adım: 5, 7'den küçük olduğu için 7'nin soluna eklenir. (Rootun solunda 5 bulunur)
3.Adım: 1, 5'ten küçük olduğu için 5'in soluna eklenir.
4.Adım: 8, 7'den büyük olduğu için 7'nin sağına eklenir. (Rootun solunda 8 bulunur)
5.Adım: 3, 1'den büyük olduğu için 1'in sağına eklenir.
6.Adım: 6, 5'ten büyük olduğu için 5'in sağına eklenir.
7.Adım: 0, 1'den küçük olduğu için 1'in soluna eklenir.
8.Adım: 9, 8'den büyük olduğu için 8'in sağına eklenir.
9.Adım: 4, 3'ten büyük olduğu için 3'ün sağına eklenir.
10.Adım: 2, 3'ten büyük olduğu için 3'ün sağına eklenir.
```

### Sonuç:
```
         7
       /   \
     5       8
    / \       \
   1   6       9
  / \
 0   3
    / \
   2   4
```
