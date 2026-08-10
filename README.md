# Kamalyse

**Arbitrage et rentabilité sur Dofus 3.6.**

Un calculateur qui répond à une seule question, déclinée par activité : *est-ce que ça vaut le
coup, et combien ça rapporte réellement ?*

L'accès est protégé par mot de passe. Pas le mot de passe ? Contacter **Ho-nimb** sur **Tylezia**.

---

## Ce que fait l'outil

Dofus regorge de conversions à taux fixe : tant de pépites pour tel objet, trois runes base pour
une Pa, une offrande contre des kamas. Ces taux sont publics et stables. Ce qui bouge, c'est le
prix HDV — et c'est là que se loge la marge.

Kamalyse met les deux bouts ensemble : le taux fixe d'un côté, ton prix de marché de l'autre, et
sort le bénéfice net, taxe de vente déduite.

## Les onglets

| Onglet | La question à laquelle il répond |
|---|---|
| **Prix** | La base commune. Tous les objets de l'outil, un seul prix par objet. |
| **Reflet Onirique** | Ce que coûte une rune de sort, et ce qu'elle rapporte revendue. |
| **Pépite** | Ce que les PNJ et le métier Mineur donnent contre des pépites. |
| **Kolizéton** | Ce que rend une Bourse une fois ses jetons dépensés. |
| **Recyclage** | Combien te coûte une pépite selon la ressource recyclée. |
| **Zones** | Que faire de tes jetons de zone : kama de glace, orichor, aviton, aliton, gladiaton. |
| **Runes** | Faut-il fusionner en Pa, en Ra, ou vendre en l'état. |
| **Élevage** | Combien payer une monture sans y perdre. |
| **Familier** | Jusqu'où monter un familier, et avec quoi le nourrir. |
| **Almanax** | L'offrande du jour, son coût réel et son bénéfice. |

## Une seule base de prix

Un prix saisi n'importe où vaut partout. Le Cœur Gelé renseigné dans Recyclage se retrouve dans
Zones, dans Familier et dans Prix, sans double saisie.

Les noms sont normalisés avant comparaison — accents, casse, ligatures. « Bidoche Goutue » et
« Bidoche Goûtue » désignent bien le même objet, quelle que soit la source qui les fournit.

Tout est stocké dans le navigateur. Rien ne part sur un serveur, il n'y a pas de compte, pas de
base de données, pas de suivi. Les boutons **Exporter** et **Importer** déplacent la base d'un
appareil à l'autre.

## Quelques calculs qui ne vont pas de soi

**Le meilleur achat n'est pas celui à la plus grosse marge.** À budget fixe, un objet peu cher
s'achète en plus grande quantité. Sur 1 M de kamas, le Galet cramoisi rapporte 3 410 000 quand le
Galet rutilant, à marge unitaire 5,7 fois supérieure, n'en sort que 1 940 000.

**Monter un familier au niveau 100 n'est pas toujours rentable.** Le palier 80 demande 29 912 XP,
le 100 en demande 179 592 — six fois plus. L'outil chiffre les trois paliers de revente et retient
le plus profitable.

**Le recyclage a un sens unique.** Une pépite s'obtient en recyclant, jamais l'inverse : le PNJ
qui vend l'Andésite 1 500 pépites ne la reprend que pour 0,4. L'arbitrage ne va que dans un sens.

**La fusion de runes est à taux fixe.** Trois base font une Pa, trois Pa font une Ra — une Ra vaut
donc neuf bases. Dès que le marché paie un palier plus cher que son équivalent en bases, il y a
une marge.

## D'où viennent les données

- **[DofusDB](https://dofusdb.fr)** — objets, icônes, échanges PNJ (`npc-shop`), rendements de
  recyclage (`recyclingNuggets`).
- **[dofusdu.de](https://api.dofusdu.de)** — calendrier Almanax, offrandes et bonus quotidiens.
- **[dafous.app](https://dafous.app/pet-xp)** — table d'XP de nourrissage des familiers. Ces
  valeurs ne figurent pas dans les données client : un seul objet du jeu, la Croquette enrichie,
  porte un effet d'XP familier.

Les catalogues se chargent à la demande et restent en cache. Un jeu de données réduit est
embarqué dans le fichier pour que l'outil soit utilisable sans réseau.

## Technique

Un seul fichier HTML. Pas de dépendance, pas d'étape de compilation, pas de serveur.

---

Projet non officiel, sans lien avec Ankama. DOFUS est une marque d'Ankama.
