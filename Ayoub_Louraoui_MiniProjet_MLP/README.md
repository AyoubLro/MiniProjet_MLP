\# Mini-projet MLP - Classification Fashion-MNIST



\## Auteur

\- Nom : Ayoub Louraoui

\- Groupe : 4IADM G1

\- Date : 18 - MARS - 2026



\---



\## Description



Ce projet implémente un Perceptron Multicouche (MLP) pour la classification d'images Fashion-MNIST



\## Contenu du dossier



Ayoub\_Louraoui\_MiniProjet\_MLP/

├── codecomplet\_MLP.ipynb # Fichier de code

├── README.md # Ce fichier

├── Rapport\_MLP.pdf # Le Rapport de ce mini projet

└── figures/ # Dossier des graphs

&#x20;    ├── accuracy\_vs\_epochs.png

&#x20;    ├── accuracy\_vs\_hiddens.png

&#x20;    ├── accuracy\_vs\_lr.png

&#x20;    └── under\_overfitting.png





\---



\## Résultats principaux



\### 1. Impact du nombre de neurones cachés



| num\_hiddens | Test Accuracy |

|-------------|---------------|

| 32 | 80% |

| 64 | 84% |

| 128 | 86% |

| 256 | 88% |

| 512 | 87% |



\### 2. Impact du learning rate



| Learning Rate | Test Accuracy |

|---------------|---------------|

| 0.001         | 75%           |

| 0.01          | 83%           |

| 0.1           | 88%           |

| 0.5           | 85%           |



\### 3. Configuration optimale



| Paramètre     | Valeur |

|---------------|--------|

| num\_hiddens   | 256    |

| learning\_rate | 0.1    |

| batch\_size    | 256    |

| epochs        | 10     |

| activation    | ReLU   |

| Test Accuracy | 88%    |



\---



\## Diagnostics



| Problème     | Configuration | Symptôme                    |

|--------------|---------------|-----------------------------|

| Underfitting | h=16          | Train=65%, Test=64%         |

| Overfitting  | h=512         | Train=94%, Test=87%, Gap=7% |

| Optimal      | h=256         | Train=91%, Test=88%, Gap=3% |



\---



\## Graphiques générés



| Fichier | Description |

|---------------------------------|----------------------------------------------------|

| `accuracy\\\\\\\_vs\\\\\\\_epochs.png`  | Évolution train/test accuracy par epoch            |

| `accuracy\\\\\\\_vs\\\\\\\_hiddens.png` | Test accuracy en fonction de num\_hiddens           |

| `accuracy\\\\\\\_vs\\\\\\\_lr.png`      | Test accuracy en fonction du learning rate         |

| `under\\\\\\\_overfitting.png`      | Comparaison underfitting vs optimal vs overfitting |

