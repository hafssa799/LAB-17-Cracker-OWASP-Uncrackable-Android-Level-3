# LAB-17-Cracker-OWASP-Uncrackable-Android-Level-3


## Étape 1 : Analyse statique simple avec Jadx-GUI (comprendre le Java)

<img width="724" height="474" alt="7" src="https://github.com/user-attachments/assets/8319986b-0d42-405c-82b6-529b21c390e3" /><img width="960" height="495" alt="2" src="https://github.com/user-attachments/assets/53f35d3d-9e6a-4327-84f9-804f5c56d365" />

<img width="602" height="181" alt="image" src="https://github.com/user-attachments/assets/eae851b5-653a-48b0-b242-caa23848e517" />

<img width="952" height="500" alt="1" src="https://github.com/user-attachments/assets/fe84486e-4a08-49e8-ade2-1e1003477f85" />

<img width="960" height="495" alt="2" src="https://github.com/user-attachments/assets/6e3a8ea2-336f-43f1-b1f3-d33cd26686d4" />

## Étape 2 : Décompiler l’APK avec apktool

<img width="488" height="153" alt="3" src="https://github.com/user-attachments/assets/9621e68d-269d-4a26-986e-4a8bc484d700" />

<img width="758" height="277" alt="4" src="https://github.com/user-attachments/assets/83753ecd-f846-4ff0-a54f-4e525bdae5e6" />

## Étape 3 : Patch smali – Supprimer le message « tampered » / root

### 1. Ouvrir le bon fichier

<img width="910" height="473" alt="5" src="https://github.com/user-attachments/assets/cb8970d3-cf70-4e9c-95e6-2689484504d2" />


### 2. Chercher le bloc d’erreur (Ctrl + F)

<img width="689" height="430" alt="6" src="https://github.com/user-attachments/assets/439cb018-fefb-4035-9e7f-98d92a4372d3" />

### 3. Le bloc exact à modifier


<img width="724" height="474" alt="7" src="https://github.com/user-attachments/assets/b85e06ed-2229-4b25-a263-2054577c4e3a" />


### 4. Deux méthodes de patch

<img width="883" height="494" alt="28" src="https://github.com/user-attachments/assets/a9732aa2-00bb-421a-848f-39bb8137b129" />

<img width="728" height="437" alt="9" src="https://github.com/user-attachments/assets/ef9ff3b6-8b8d-48d8-8550-42635e6f185f" />

### 5. Sauvegardeur

### 6. Recompiler l’APK

<img width="947" height="136" alt="image" src="https://github.com/user-attachments/assets/1a8655df-9666-44a4-a0f9-68ec932d8785" />

### 7. Signer l’APK

<img width="644" height="361" alt="image" src="https://github.com/user-attachments/assets/5ec29bd2-9723-42d2-bd5c-b000dfa512c8" />

### 8. Installer et tester

<img width="591" height="340" alt="image" src="https://github.com/user-attachments/assets/e1caab08-30de-4bbb-9f39-a0d3b9ea335d" />

<img width="216" height="360" alt="image" src="https://github.com/user-attachments/assets/520984e3-9e54-4df6-b7f9-eb486f41670f" />

### Étape 4 : Patch de la librairie native avec Ghidra

<img width="1422" height="753" alt="image" src="https://github.com/user-attachments/assets/dbe82925-3009-4dee-8e4e-97d1cb1baf2b" />

<img width="947" height="449" alt="image" src="https://github.com/user-attachments/assets/d3e3aeaa-5b4d-4980-b06e-95b61eea1d25" />

### Étape 5 : Analyser la logique native de vérification dans libuncrackable3.so

#### 1. Revenir au point d’entrée Java

<img width="1320" height="414" alt="image" src="https://github.com/user-attachments/assets/45c63ae4-f5ad-4681-b6af-34f2ecb7769c" />

#### 2. Retrouver la fonction native correspondante

<img width="811" height="667" alt="image" src="https://github.com/user-attachments/assets/d5bcf09c-e2c5-4687-88ad-f8d0ebf2661e" />

#### 3. Observer la structure générale du pseudo-code

<img width="1917" height="966" alt="image" src="https://github.com/user-attachments/assets/a390591a-47ab-469c-b343-a03fd83eff97" />

#### 4. Vérification avec l'installation et tester

<img width="423" height="203" alt="image" src="https://github.com/user-attachments/assets/fabb6e34-83b0-468c-a03e-0d29eda7b9f5" />
