# Virágfajok felismerése gépi tanulással

## Projekt leírás

A projekt célja egy olyan gépi tanulási modell létrehozása, amely képes különböző virágfajokat felismerni képek alapján. A feladat során egy konvolúciós neurális hálózatot (CNN) alkalmaztunk a képosztályozási probléma megoldására.

A projekt a CRISP-DM adatelemzési módszertant követi, amely strukturált megközelítést biztosít az adatok elemzéséhez és a modellek fejlesztéséhez.

---

## Adatforrás

A projektben használt adathalmaz a Kaggle platformról származik:

https://www.kaggle.com/code/siddp6/flower-images-classification

A dataset 5 különböző virágfajt tartalmaz:

- százszorszép (daisy)
- pitypang (dandelion)
- rózsa (roses)
- napraforgó (sunflowers)
- tulipán (tulips)

Az adatok mappastruktúrában vannak tárolva, ahol minden virágfaj külön könyvtárban található.

---

## Alkalmazott módszerek

A projekt során a következő Python könyvtárakat használtuk:

- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Pillow

A képek egységes méretre lettek átméretezve (180×180 pixel), majd tanító és validációs halmazra lettek bontva.

---

## Modell

A virágok felismeréséhez konvolúciós neurális hálózatot (CNN) alkalmaztunk.

A projekt során több modell architektúrát is teszteltünk:

- egyszerű CNN modell
- CNN modell dropout réteggel

A modellek teljesítményét validációs pontosság alapján hasonlítottuk össze.

---

## Vizualizációk

A projekt során többféle adatvizualizáció készült:

- kategóriaeloszlás grafikon
- képméret hisztogramok
- tanulási görbék (accuracy és loss)
- confusion matrix
- predikció valószínűségi grafikon

Ezek segítettek megérteni a dataset szerkezetét és a modell működését.

---

## Modell kiértékelése

A modell teljesítményét a következő módszerekkel értékeltük:

- validációs pontosság
- tanulási görbék elemzése
- confusion matrix

A confusion matrix segítségével azonosítottuk a legnehezebben felismerhető virágfajokat.

---

## Modell használata

A végső modell lehetővé teszi, hogy a felhasználó egy új virágképet töltsön fel, amelyen a modell predikciót végez.

A predikció során:

- a kép feldolgozásra kerül
- a modell kiszámítja az egyes kategóriák valószínűségét
- a rendszer megjeleníti a legvalószínűbb virágfajt és a predikció megbízhatóságát

---

## Projekt struktúra

```
adatelemzesi-projekt/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── models/
├── video/
├── README.md
├── environment.yml
├── .gitignore
└── requirements.txt
```

## Fejlesztési lehetőségek

A modell teljesítménye több módon javítható:

- nagyobb és változatosabb dataset használata
- data augmentation alkalmazása
- mélyebb neurális háló architektúrák használata
- transfer learning alkalmazása (pl. MobileNet, ResNet)
- több epoch használata a tanítás során

---

## Következtetés

A projekt során sikeresen létrehoztunk egy működő képosztályozó modellt, amely képes különböző virágfajokat felismerni. Az eredmények azt mutatják, hogy a konvolúciós neurális hálózatok hatékonyan alkalmazhatók képfelismerési feladatokban.
