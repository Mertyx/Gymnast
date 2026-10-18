# 01 – Ideový plán projektu

## 1. Formální Název projektu
**SwingDoll: Physics Gymnast**

---

## 2. Marketingový úvodník
Chceš si vyzkoušet, jaké to je být akrobatem na hrazdě, ale nemáš fyzičku a bojíš se, že si zlámeš vaz? SwingDoll je chytlavá 2D ragdoll hra, kde rozhoduje jen tvoje načasování a cit pro fyziku. Rozhoupej se na tyči, chyť rytmus, udělej Salto a dopadni jako profík! Jednoduché ovládání, ale brutální zábava na hodiny.

---

## 3. Popis hry
* **Základní principy:** Hráč ovládá postavičku (stickmana) složenou z ragdoll kloubů. Postava reaguje na gravitační sílu a setrvačnost.
* **Funkčnost a možnosti:**
  * **Chytání/Pouštění tyče:** Stiskem klávesy se ruka přichytí k najbližší tyči. Pustěním klávesy se hráč vymrští do vzduchu.
  * **Ovládání těla (Tuck & Arch):** Pomocí dalších kláves může hráč tělo buď zkrčit (kolena k hrudníku pro rychlejší rotaci) nebo prohnout/natáhnout (pro nabrání švihu).
  * **Fyzikální ragdoll:** Při nárazu do překážky nebo pádů na zem tělo nereaguje animací, ale reálnou simulací pádu.
* **Cíle hráče:**
  * Překonat danou trať s tyčemi od startu až do cílové dopadové zóny.
  * Získat co nejvyšší skóre za počet přetočení (flipů) ve vzduchu a čistotu dopadu.

---

## 4. Popis audiovizuálu
* **Vizuální styl:**
  * Čistý, minimalistický 2D flat design / pixel-art.
  * Postava je jednoduchý Stickman (černé čáry a kruh jako hlava), aby vynikla samotná fyzika pohybu.
  * Pozadí tvoří jednoduchá městská nebo tělocvičná scéna s kontrastními tyčemi.
* **Audio:**
  * **Zvuky:** Jednoduché efekty (SFX) pro chycení tyče (cvaknutí), švih vzduchem (whoosh efekt) a legrační zvuk při tvrdém dopadu na zem.
  * **Hudba:** Lo-fi nebo energický synth-wave podkres na pozadí, který neruší při soustředění.

---

## 5. Chystané použité technologie
* **Game Engine:** Godot Engine 4.x (využití vestavěného 2D physics enginu – `RigidBody2D`, `PinJoint2D`, `Area2D`).
* **Jazyk:** GDScript.
* **Verzování:** Git + GitHub.
* **Grafika:** Aseprite / Inkscape 
* **Audio:** BFXR / Audacity na úpravu zvuků.

---

## 6. Hypotézy projektu
1. **Hypotéza 1 (Hratelnost):** Hráči pochopí princip ovládání švihu a krčení těla (Tuck/Arch) do 30 sekund od spuštění hry bez nutnosti číst dlouhý tutoriál.
2. **Hypotéza 2 (Zábavnost pádu):** Díky ragdoll fyzice budou hráče bavit i neúspěšné pokusy a pády, což sníží frustraci z obtížnosti a donutí je hrát znovu (tzv. "ještě jeden pokus" efekt).
