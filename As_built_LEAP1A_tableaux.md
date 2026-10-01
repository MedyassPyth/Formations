# As-built LEAP 1A — conversion du XML en tableaux

Source : [xml as-built.txt](./xml%20as-built.txt), dépôt `MedyassPyth/Formations`. Empreinte du fichier source (SHA Git) : `51c4d03a3cbbef5309f105a154f544c1aaaca649`.

## 1. Données générales de l’as-built

### Transmission

| Champ XML | Libellé | Valeur |
| --- | --- | --- |
| `RECORD_FILE_TYPE` | Type d’enregistrement | AHDR |
| `SENDER_CODE` | Code émetteur | TA |
| `SENDING_DATE` | Date d’envoi | 2016-05-13 |

### Ensemble parent

| Champ XML | Libellé | Valeur |
| --- | --- | --- |
| `RECORD_FILE_TYPE` | Type d’enregistrement | BASA |
| `ITEM_SERIAL_NUMBER` | Numéro de série | MC053316 |
| `MP_NAME` | Référence de l’ensemble | 362-000-310-0 |
| `MP_STATUS` | Statut de l’ensemble (code brut) | R |
| `SB_ENGINE_MARK_NUMBER` | Désignation du programme moteur | LEAP 1A |
| `CLASSIFIED_MASTERPART` | Indicateur CLASSIFIED de l’ensemble | YES |
| `RECONCILIATION_DATE` | Date de réconciliation | 2016-05-13 |
| `MP_TITLE` | Titre de l’ensemble | MC053316 |
| `EDD_REFERENCE` | Référence EDD | W2A556G0010 |
| `RECONCILIATION_SIGNATURE` | Signature de réconciliation (valeur brute) | TA |
| `ASSEMBLY_RESPONSIBILITY` | Responsabilité de montage | TA |
| `ACTUAL_PC_DATA` | ACTUAL_PC_DATA (code brut) | TA |
| `SUPPLY_RESPONSIBILITY` | Responsabilité de fourniture | TA |
| `TARGET_PC_DATA` | TARGET_PC_DATA (code brut) | TA |
| `SN_REPERE_FONCTIONNEL` | Repère fonctionnel | 81000 |

### Structure XML

La racine `ASBUILT_TRANSMISSION` contient `AB_HEADER`, puis `AB_MASTERPART`, puis les blocs `AB_COMPONENT`. Les 43 lignes ci-dessous sont toutes des enfants directs du même ensemble parent, numéro de série **MC053316**, référence **362-000-310-0**.

| Propriété XML | Valeur |
| --- | --- |
| Version XML | 1.0 |
| Encodage déclaré | UTF-8 |
| Espace de noms par défaut | `snm.XMLSchema.ASBUILT` |
| Espace de noms du préfixe ab | `snm.XMLSchema.ASBUILT.common` |
| Espace de noms du préfixe xsi | `http://www.w3.org/2001/XMLSchema-instance` |

## 2. Tableau des composants

Une ligne correspond à un bloc `AB_COMPONENT`, dans l’ordre du XML. Les références répétées sont conservées : elles peuvent correspondre à des repères fonctionnels différents. La colonne « Ligne » est ajoutée pour faciliter le repérage. « Absent » signifie que la balise n’existe pas dans le bloc source. « Vide » signifie qu’une balise est présente sans valeur.

| Ligne | Référence (PART_NUMBER) | Désignation (PART_TITLE) | N° de série (ITEM_SERIAL_NUMBER) | Quantité (QUANTITY) | Repère (SN_REPERE_FONCTIONNEL) | Date montage (SN_DATE_ASSEMBLY) | CLASSIFIED_PART_INDICATOR |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 362-504-901-0 | GICLEUR,JRS | Absent | 1 | 815B0 | 2016-05-13 | NO |
| 2 | AS3209-010 | PACKING | Absent | 1 | 815N3 | 2016-05-13 | NO |
| 3 | J626P04 | NUT, SELF-LOCK | Absent | 1 | 812K2 | 2016-05-13 | NO |
| 4 | 362-045-301-0 | ROUE PHONIQUE | Absent | 1 | 810A2 | 2016-05-13 | NO |
| 5 | 362-045-710-0 | FREIN ECROU | Absent | 1 | 810E0 | 2016-05-13 | NO |
| 6 | 362-503-310-0 | SUPPORT,PALIER 1 | MA480818 | 1 | 815A0 | 2016-05-13 | YES |
| 7 | 362-905-901-0 | ROULEMENT DE PALIER 1 | HF741716 | 1 | 811A0 | 2016-05-13 | YES |
| 8 | J626P04 | NUT, SELF-LOCK | Absent | 1 | 815K6 | 2016-05-13 | NO |
| 9 | 362-046-701-0 | DISQUE DECOUPLEUR | Absent | 1 | 810A1 | 2016-05-13 | NO |
| 10 | 362-046-901-0 | SEGMENT ETANCHEITE | Absent | 2 | 811P0 | 2016-05-13 | NO |
| 11 | 362-048-001-0 | JOINT RADIAL SEGMENTE | DV132500 | 1 | 815P0 | 2016-05-13 | YES |
| 12 | 362-048-501-0 | ECROU, BAGUE INT PALIER 2 | Absent | 1 | 812K1 | 2016-05-13 | NO |
| 13 | 362-504-810-0 | TUBE,ALIM FILM HLE PAL 1 | Absent | 1 | 815B2 | 2016-05-13 | NO |
| 14 | AS3237-28 | VIS | Absent | 8 | 815F2 | 2016-05-13 | NO |
| 15 | 362-024-710-0 | LABYRINTHE TOURNANT,PALIER 1 | Absent | 1 | 811A1 | 2016-05-13 | NO |
| 16 | 362-503-402-0 | SUPPORT,PALIER 2 | MA415217 | 1 | 815A1 | 2016-05-13 | YES |
| 17 | 650-365-095-0 | ANNEAU ARRET | Absent | 1 | 815W1 | 2016-05-13 | NO |
| 18 | AS3209-010 | PACKING | Absent | 1 | 815N5 | 2016-05-13 | NO |
| 19 | AS3217-215 | ANNEAU ELASTIQUE | Absent | 1 | 810W0 | 2016-05-13 | NO |
| 20 | AS3217-244 | ANNEAU ELASTIQUE | Absent | 1 | 811W0 | 2016-05-13 | NO |
| 21 | 362-045-020-0 | ARBRE DE COMPRESSEUR BP | HD106225 | 1 | 810A0 | 2016-05-13 | YES |
| 22 | 362-048-402-0 | ECROU,BAGUE EXT PALIER 2 | Absent | 1 | 812K0 | 2016-05-13 | NO |
| 23 | 362-048-901-0 | RONDELLE, VIS FUSIBLE | Absent | 20 | 815J0 | 2016-05-13 | NO |
| 24 | 362-503-201-0 | FLASQUE ETANCHEITE PALIER | Absent | 1 | 815A2 | 2016-05-13 | NO |
| 25 | 649-784-524-0 | NUT | Absent | 20 | 815K0 | 2016-05-13 | NO |
| 26 | 649-786-821-0 | ANNEAU D'ARRET | Absent | 1 | 812W0 | 2016-05-13 | NO |
| 27 | AS3237-08 | BOLT MACHINE DHH | Absent | 1 | 815F3 | 2016-05-13 | NO |
| 28 | 362-045-510-0 | FREIN ECROU,DE PALIER 1 | Absent | 1 | 811E0 | 2016-05-13 | NO |
| 29 | 362-501-401-0 | JOINT TORIQUE FLASQUE | Absent | 1 | 815N0 | 2016-05-13 | NO |
| 30 | AS3209-010 | PACKING | Absent | 1 | 815N2 | 2016-05-13 | NO |
| 31 | J626P04 | NUT, SELF-LOCK | Absent | 6 | 815K1 | 2016-05-13 | NO |
| 32 | J626P04 | NUT, SELF-LOCK | Absent | 8 | 815K2 | 2016-05-13 | NO |
| 33 | J626P04 | NUT, SELF-LOCK | Absent | 1 | 815K5 | 2016-05-13 | NO |
| 34 | J814P008A | BOLT MACHINE DHH | Absent | 1 | 815F5 | 2016-05-13 | NO |
| 35 | 362-046-402-0 | ROULEMENT DE PALIER 2 | DV738727 | 1 | 812A0 | 2016-05-13 | YES |
| 36 | 362-046-810-0 | ECROU ENCOCHE ARRIERE,CBP | Absent | 1 | 810K0 | 2016-05-13 | NO |
| 37 | AS3237-12 | VIS | Absent | 6 | 815F1 | 2016-05-13 | NO |
| 38 | AS3237-18 | BOLT MACH D HEX E WASH HEAD | Absent | 1 | 812F0 | 2016-05-13 | NO |
| 39 | 362-024-504-0 | VIS FUSIBLE | Absent | 20 | 815F0 | 2016-05-13 | NO |
| 40 | 362-045-601-0 | FREIN ECROU, DE PALIER 2 | Absent | 1 | 812E0 | 2016-05-13 | NO |
| 41 | 362-081-801-0 | CHEMINEE DESHUILEUR | Absent | 24 | 810E1 | 2016-05-13 | NO |
| 42 | 362-501-501-0 | JOINT TORIQUE INTER SUPPORT | Absent | 1 | 815N1 | 2016-05-13 | NO |
| 43 | AS3209-274 | JOINT TORIQUE | Absent | 2 | 815N4 | 2016-05-13 | NO |

### Champs communs aux 43 lignes

Ces champs sont identiques dans tous les blocs composants. Ils sont présentés une seule fois pour garder le tableau lisible et conserver l’ensemble des données source.

| Champ XML | Valeur commune | Présence |
| --- | --- | --- |
| `RECORD_FILE_TYPE` | FASC | 43 / 43 blocs |
| `LOOSE_PART_CODE` | 0 | 43 / 43 blocs |
| `ASSEMBLY_RESPONSIBILITY` | TA | 43 / 43 blocs |
| `SUPPLY_RESPONSIBILITY` | Vide | 43 / 43 blocs |
| `SN_BLADE_POSITION` | Vide | 43 / 43 blocs |
| `SN_BLADE_MOMENT_WEIGHT` | Vide | 43 / 43 blocs |
| `SN_INDIC_MANQUANT` | NO | 43 / 43 blocs |
| `SN_CODE_PRODUCTEUR_RELEVE` | F0301 | 43 / 43 blocs |

### Correspondance des colonnes

| Colonne | Champ XML |
| --- | --- |
| Ligne | Ajout de conversion : ordre du bloc dans le XML |
| Référence | `PART_NUMBER` |
| Désignation | `PART_TITLE` |
| N° de série | `ITEM_SERIAL_NUMBER` |
| Quantité | `QUANTITY` |
| Repère | `SN_REPERE_FONCTIONNEL` |
| Date montage | `SN_DATE_ASSEMBLY` |
| CLASSIFIED_PART_INDICATOR | `CLASSIFIED_PART_INDICATOR` |

## 3. Synthèse de l’exemple

| Indicateur | Valeur |
| --- | --- |
| Ensembles parents | 1 |
| Blocs composants | 43 |
| Références distinctes | 37 |
| Blocs avec numéro de série renseigné | 6 |
| Blocs sans balise de numéro de série | 37 |
| Blocs avec SN_INDIC_MANQUANT = NO | 43 |

## 4. Précisions de lecture

- Cet exemple porte sur le **LEAP 1A**. Il ne suffit pas à établir le format applicable au M88.
- L’absence de numéro de série dans un bloc ne permet pas, à elle seule, de distinguer un composant loti d’un composant suivi uniquement par référence. Aucun champ de lot n’apparaît dans cet exemple.
- Les valeurs `R`, `TA`, `F0301`, `BASA`, `FASC`, `AHDR` et `0` sont conservées telles quelles. Leur signification métier doit être confirmée par la spécification d’interface.
- Les indicateurs `CLASSIFIED_MASTERPART` et `CLASSIFIED_PART_INDICATOR` sont conservés sans les assimiler à une catégorie de sécurité ou de traçabilité.
- Les champs `SN_BLADE_POSITION` et `SN_BLADE_MOMENT_WEIGHT` sont présents mais vides pour toutes les lignes.
- `RECONCILIATION_SIGNATURE` appartient à l’ensemble parent. Ce fichier ne précise pas si cette valeur constitue un visa opérateur ni ce qu’elle engage.
- Aucun bloc d’opération, d’étape, d’instruction de travail, de résultat de contrôle ou d’historique de démontage/remontage n’est présent dans cet exemple.

La conversion conserve tous les champs et toutes les valeurs des blocs d’en-tête, de l’ensemble parent et des composants. Les champs communs sont factorisés dans leur tableau dédié.
