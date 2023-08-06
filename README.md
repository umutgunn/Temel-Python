# Temel-Python

* 1- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir.

```def flat(l):
    flatten =[]
    for i in l:
        if type(i) != list:
            flatten.append(i)
        else:
            flatten.extend(flat(i))
    return flatten
```

* 2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün.

```def rev(l):
    l.reverse()
    for i in l:
        if type(i) == list:
            i.reverse()    
    return l
```
