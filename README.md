ExxonMobil Implied Vol YahooFinance : 
-	Def Calcule CDF de la loi normale pour calculer prix options dans BS
-	Def Formule BS qui retourne le prix de l’option
-	Def Calcule la volatilite implicite pour que BS price = price via dichotomie
-	Def Récupérer le spot du sous-jacent le plus proche 
-	Trouver l’option la plus ATM parmis le choix et choisir le prix de l’option via mid ou last price du trade  
-	Def construire un dataset de volatilités implicites en utilisant toutes les options du sous-jacent et et pour chaque expiry date, on choisit le prix mid pour le call et le put . On calcule iv via implied_vol_bisect de chaque option … si échec, utilise impliedVolatility fourni par Yahoo. Iv entre 1e-4 et 2.0. 
-	Def Afficher la surface IV 3D. 
-	Cette fonction cherche une expiry proche de target_days qui renvoie une chain exploitable.Yahoo bug parfois : certaines expiries renvoient une chaîne vide, ou plantent.
-	Prendre un snapshot : spot + prix du call ATM + prix du put ATM, pour UNE expiry
-	Execute(appelle les fonctions pour) les surfaces IV call et put 
-	Execute(appelle les fonctions pour) prix call et put ainsi que mon spot toutes les minutes.
<img width="454" height="405" alt="image" src="https://github.com/user-attachments/assets/5326bda9-e37a-4cfe-a9da-07ac6951ccca" />
