# **Proje 2**
## Soru
 a) [16,21,11,8,12,22] dizisini <span style="color: red;"> Merge Sort </span> algoritmasına göre aşamalarını yazınız.
 b) <span style="color: red;">Big-O</span> gösterimini yapınız.
***
## Cevap ##
 a) Divide and Conquer
 * [16,21,11] <----> [8,12,22]
 * [16] <----> [21,11] / [8,12] <----> [22]
 * [16] / [21] <----> [11] / [8]<---->[12] / [22]
 * [16] / [21] / [11] / [8] / [12] / [22]
***
Merge
* [16] / [11,21] / [8,12] / [22]
 * [11,16,21] / [8,12,22]
 * [8,11,12,16,21,22]

b) Verilen diziyi ortadan ikiye böleriz. Bu işlem log(n) adımda gerçekleşir, çünkü her seferinde dizi ikiye bölünür.Birleştirme adımı, iki sıralı alt diziyi birleştirirken elemanları karşılaştırır ve sıralı bir şekilde birleştirir. Bu işlem, her alt dizi için O(n) zaman alır. Toplamda, bölme adımında log(n) kez bölündüğü için birleştirme adımı O(n*logn) zaman karmaşıklığına sahiptir.