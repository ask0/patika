# Proje 1

**[22,27,16,2,18,6]** -> Insertion Sort

**_Q: Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız._**

```
[22,27,16,2,18,6]

[16,22,27,2,18,6]

[2,16,22,27,18,6]

[2,16,18,22,27,6]

[2,6,16,18,22,27]
```

**1.** Insertion sort için öncelikle verilen array'i 2 parçaya ayırırız; ilk eleman (sıralı alan) ve kalan elemanlar (sıralanmamış alan). Ardından sıralanmamış alanın ilk elemanına bakılır ve sıralanmış alanda nereye eklenmesi gerektiğini sol komşusuyla karşılaştırarak kontrol edilir.

**2.** Bu örnekte sıralı alanın ilk elemanı 22, sıralanmamış alanın ilk elemanı 27.

**3.** 27, 22'nin sağında olması gerektiği için sıralı alanlarda bir yer açıp 27'yi 22'nin sağına ekleriz.

**4.** Bu adımdaki sıralı alan: **22,27** | Sıralı olmayan alan: **16,2,18,6** olmuş olur.

**5.** Sıralı olmayan alandaki ilk eleman: 16

Sol komşularıyla kıyaslarsak, 16 sayısı listenin en başına gelir. Son durum: **16,22,27**

**6.** Sıralı olmayan alanda eleman kalmayana dek bir önceki adım tekrar edilir.

---

**_Q: Big-O gösterimini yazınız._**

```
A: n elemanlı bir dizi için (n-1) kaydırma işlemi gerçekleşir. Sıralama için yapılan karşılaştırma ve kaydırma işlemlerini hesaplarsak, n(n-1)= n^2-1

O(n^2)
```

---

**_Q: Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?_**

- Average case: Aradığımız sayının ortada olması
- Worst case: Aradığımız sayının sonda olması
- Best case: Aradığımız sayının dizinin en başında olması.

```
18 elemanı dizinin ortasında olduğu için Average Case kapsamına girer.

Average Case: O(n^2)
```

**_Q: [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız._**

```
[2,3,5,8,7,9,4,15,6]
[2,3,5,8,7,9,4,15,6]
[2,3,4,8,7,9,5,15,6]
[2,3,4,5,7,9,8,15,6]
```
