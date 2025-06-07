# 📸 Capture d'écran 4K parfaite d'un CV HTML/CSS (quand l'impression en PDF échoue)

J'ai créé mon CV en utilisant **HTML** et **CSS Grid**, et je voulais l'exporter en **PDF** propre et professionnel.  
Mais tous les outils que j'ai essayés — impression navigateur, Puppeteer, extensions de capture d'écran — ont échoué à rendre la mise en page correctement.  
Le texte était flou, les éléments bougeaient, et le design était cassé.

---

## ❌ Le Problème

J'ai tout essayé :

-   **Chrome "Imprimer en PDF"** → mise en page décalée, polices floues
-   **Outils de capture d'écran en ligne** → artefacts de compression, styles perdus
-   **Générateurs PDF (Puppeteer, extensions)** → CSS Grid et Flexbox cassés
-   **OBS / captures d'écran système** → pas assez nets pour zoomer ou partager
    Quand vous utilisez des **mises en page modernes (Grid, Flexbox)** avec un espacement et alignement précis, ces méthodes peuvent facilement ruiner la fidélité visuelle de votre CV.

---

## ✅ La Solution

La solution que j'ai trouvée ?  
Prendre une **capture d'écran haute résolution directement depuis Chrome DevTools** en utilisant un appareil personnalisé avec un **ratio de pixels d'appareil** (DPR) élevé.  
Cette approche préserve chaque détail exactement comme rendu dans votre navigateur.

---

### 💡 Pourquoi ça marche

-   Rend votre CV comme un vrai navigateur (pas de bizarrerie de feuille de style d'impression)
-   Conserve les **polices nettes** et la mise en page **CSS Grid/Flexbox** précise
-   Résolution et mise à l'échelle entièrement personnalisables
-   Produit une **image PNG** sans perte — parfaite pour la conversion ou l'impression

---

## 🛠️ Guide étape par étape

1. Ouvrez votre CV dans **Google Chrome**
2. Appuyez sur `Ctrl + Shift + I` (ou `Cmd + Option + I` sur Mac) pour ouvrir **DevTools**
3. Appuyez sur `Ctrl + Shift + M` pour basculer en **Mode Design Responsive**
4. Cliquez sur le menu déroulant des appareils > **Modifier...** > **Ajouter un appareil personnalisé**
    - Nom : `Capture 4K`
    - Largeur : `900`
    - Hauteur : `1520`
    - Ratio de pixels d'appareil : `4`
    - Type : `Bureau`
    - Laisser l'Agent utilisateur vide
    - Cliquez sur **"Ajouter"**
5. Sélectionnez `Capture 4K` dans le menu déroulant
6. Réglez le zoom à **75%** (ou ajustez selon vos besoins pour adapter le contenu)
7. (Optionnel) Rechargez la page pour vous assurer que tout se rend correctement
8. Cliquez sur le menu à trois points dans DevTools > **Capturer une capture d'écran** ou **Capturer une capture d'écran pleine taille**

---

## 📄 De la capture d'écran au PDF

Vous aurez maintenant une **image PNG cristalline** de votre CV.
Pour la convertir en PDF :

-   Utilisez [png2pdf.com](https://png2pdf.com) — glissez-déposez votre/vos fichier(s) PNG
-   Combinez plusieurs captures d'écran en un seul PDF si votre CV s'étend sur plusieurs pages
    Maintenant votre PDF ressemblera **exactement** à votre version HTML/CSS — mise en page intacte, aucune distorsion.

---

## ✨ Conseils bonus

-   Vous pouvez réutiliser cette astuce pour des portfolios, tableaux de bord, ou designs web — toute mise en page qui casse à l'impression.
-   Pour les CV multi-pages : prenez une capture d'écran par "hauteur de page" et fusionnez-les plus tard.

---

## 🙌 Réutilisation et partage

N'hésitez pas à forker ce repo! 
Si cela vous a aidé, partagez-le — cela pourrait épargner des heures de frustration à quelqu'un d'autre 😊
