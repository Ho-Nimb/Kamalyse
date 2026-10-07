# Kamalyse — calculateur de pépites et d'XP familier sur Dofus

**Combien coûte réellement une pépite selon ce que tu brises, et jusqu'où monter un familier.**

👉 **[Ouvrir le calculateur](https://ho-nimb.github.io/Kamalyse/)**

---

Dofus regorge de conversions à taux fixe : tant de pépites pour tel objet, trois runes base pour
une Pa, une offrande contre des kamas. Ces taux sont stables. Ce qui bouge, c'est le prix en hôtel
de vente — et c'est là que se loge la marge. Kamalyse met les deux bouts ensemble et sort le
bénéfice net, taxe de vente déduite.

## En accès libre

| Onglet | La question à laquelle il répond |
|---|---|
| **Recyclage** | Combien te coûte une pépite selon la ressource brisée au recycleur. Les routes sont classées de la moins chère à la plus chère, en kamas par pépite. |
| **Familier** | Jusqu'où monter un familier et avec quoi le nourrir. L'outil combine viandes et bidoches par coût croissant, puise d'abord dans ton stock, et compare les trois paliers de revente — 80, 90, 100. |

Le moteur de calcul y est entier. À toi d'y saisir tes rendements et tes prix.

## En accès complet

- le relevé complet : plus de **8 000 rendements de brisage** et **2 000 valeurs d'expérience de
  nourrissage**, déjà saisis ;
- les **prix d'hôtel de vente** relevés et nettoyés ;
- les onglets d'arbitrage : **Prix, Reflet Onirique, Pépite, Kolizéton, Zones, Runes, Élevage,
  Packs métiers, Almanax**.

👉 **[Me contacter sur Discord](https://discord.com/users/100199918261522432)**

## Quelques calculs qui ne vont pas de soi

**Le meilleur achat n'est pas celui à la plus grosse marge.** À budget fixe, un objet peu cher
s'achète en plus grande quantité : la marge unitaire la plus élevée perd souvent contre le meilleur
rendement.

**Monter un familier au niveau 100 n'est pas toujours rentable.** Les derniers niveaux coûtent
plusieurs fois le palier 80 en expérience, alors que le prix de revente, lui, ne suit pas toujours.

**Le recyclage a un sens unique.** Une pépite s'obtient en brisant, jamais l'inverse : le PNJ qui
vend un objet contre des pépites ne le reprend pas au même tarif. L'arbitrage ne va que dans un
sens.

**La fusion de runes est à taux fixe.** Trois base font une Pa, trois Pa font une Ra — une Ra vaut
donc neuf bases. Dès que le marché paie un palier plus cher que son équivalent en bases, il y a une
marge à prendre.

## Technique

Un seul fichier HTML. Pas de dépendance, pas d'étape de compilation, pas de serveur. Tout reste
dans ton navigateur : pas de compte, pas de base de données, pas de suivi. Les boutons **Exporter**
et **Importer** déplacent ta base d'un appareil à l'autre.

Données de référence : [DofusDB](https://dofusdb.fr) pour les objets, icônes et échanges PNJ,
[dofusdu.de](https://api.dofusdu.de) pour le calendrier Almanax.

---

Projet non officiel, sans lien avec Ankama. DOFUS est une marque d'Ankama.
