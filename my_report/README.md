# Lesson: Digital & Serious Games

### First and Last Name: THEODOSIS PAPADIMITRIOU
### University Registration Number: dpsd19093
### GitHub Personal Profile: https://github.com/papadimitriou19093
### Digital & Serious Games Personal Repository: xxx

# Introduction
test

# Summary


# 1st Deliverable
Αρχικά κατέβασα το unity hub και στην συνέχεια την 2019.4 έκδοση του editor. Στην συνέχεια ξεκίνησα το πρώτο μου project πάνω σε 2d template. Αφού δημιούργησα το βασικό scene και το ονόμασα main scene,  βρήκα από το google έναν χαρακτήρα τύπου pixel art ![hero_spritesheet](https://user-images.githubusercontent.com/100956248/202170625-fbe8e1fa-d741-4ddc-8680-8ba2e6ef632a.png)
 (αναζήτησα 2d character sprite sheets). Αφού το έκανα drag and drop σε έναν φάκελο που δημιούργησα στα assets του project και το ονόμασα  hero έκανα την μετατροπή σε multiple sprite mode και από τον editor χώρισα αυτόματα τις στάσεις του χαρακτήρα. Για τον χαρακτήρα δημιούργησα και ένα  animation για το περπάτημα ονομάζοντάς το walking. Τέλος μέσω του κώδικα στο visual και μέσω τον ρυθμίσεων στα project settings έφτιαξα τον χαρακτήρα μου να κινείτε με το βελάκια (πάνω, κάτω, δεξιά και αριστερά) και αφού έφτιαξα το timing και to framerate όρισα την ταχύτητα που θα κινείτε ο χαρακτήρας από τον κώδικα και πρόσθεσα το script στο inspection του χαρακτήρα. Το επόμενο βήμα μου ήταν να βρω ένα αντίστοιχο sprite sheet για το tile map που το έκανα επίσης με τον ίδιο τρόπο όπως τον χαρακτήρα ![32x32_map_tile v1 1_0](https://user-images.githubusercontent.com/100956248/202170439-8894f33d-538a-4e80-accf-790d486ba738.png)
(βρήκα ένα sprite sheet από το google το έκανα import στο project και από inspection το χώρισα σε πολλά διαφορετικά assets). Στην συνέχεια ξεκίνησα να δημιουργώ την παλέτα μου που είχε κάποια ξεχωριστά tiles αλλά και sets αυτών. ![bkkbk](https://user-images.githubusercontent.com/100956248/202172342-f07d7878-0ddc-4e2e-83e3-72d5f5c9d315.JPG)
 Μετά μεγάλωσα το μέγεθος τις κάμερας για να προσθέσω περισσότερα tilesΚαι τέλος με την βοήθεια της παλέτας αφού είχα δημιουργήσει και ένα  grid-tile map στο main scene τα πρόσθεσα στο παιχνίδι. ![kkk](https://user-images.githubusercontent.com/100956248/202172238-3e970ceb-b1c5-405e-9c0a-730601bc6541.JPG)

 Επίσης έφτιαξα και τις αναλογίες των tiles αλλά και του χαρακτήρα. Τέλος το έκανα built and run και από το GitHub Desktop έβαλα τους φακέλους για να ανέβουν στο GitHub.
 Τέλος βάζω και φωτογραφίες τον χωρισμένων assets αλλά και του χάρτη ολοκληρωμένο.
 ![assets1](https://user-images.githubusercontent.com/100956248/202172450-d7b48195-3af8-4a7f-94ca-317c2499e8cd.JPG)
![asset2](https://user-images.githubusercontent.com/100956248/202172491-a4b762c9-bba8-41b5-aad4-bfd5b94c82d0.JPG)
![Capture](https://user-images.githubusercontent.com/100956248/202172530-09b9994c-d36e-4bac-af2f-33f877502559.JPG)
Και ένα βίντεο με το παιχνίδι να παίζει μέσα στον Editor του Unity
https://user-images.githubusercontent.com/100956248/202175637-268de7eb-de97-407f-a038-549024d97a14.mp4
# 2nd Deliverable
Αρχικά επέκτεινα το tilemap και έβαλα διάφορα εμπόδια.

 Πρόσθεσα στον ήρωα το Rigid Body 2D και αλλάζοντας την τιμή gravity στο Inspector (από ένα σε 0) ο ήρωας παραμένει στον χάρτη. Πρόσθεσα στον ήρωα το Box Collider 2D και έφτιαξα απο το edit collider την ζώνη στην οποία ο ήρωας θα αλληλεπιδρά με άλλα colliders. Στην συνέχεια, έβαλα μερικά εμπόδια αφού είχα δημιουργήσει ένα prefab για αυτά και τους είχα βάλει το Box Collider 2D.

 Τώρα ο χαρακτήρας μου αλληλεπιδρά με τα εμπόδια και δεν μπορεί να πάει από πάνω τους. Έφτιαξα την περιστροφή του ήρωα παγώνοντας την περιστροφή στον z άξονα απο το Rigid Body 2D.

 ‘Αλλαξα τον κώδικα και επειδή ο ήρωάς μου ήταν αργός μετέτρεψα την void Update() σε void FixedUpdate(). Έφτιαξα και το εύρος των συγκρούσεων και για τα απλά Colliders από το edit Collider. Στο Inspector του Tilemap έβαλα το Tilemap Collider 2D και επέλεξα τα tiles που δεν θα αλληλεπιδρούν με τον ήρωα αλλάζοντας το Collider Type στο None ( από Sprite). Τέλος πρόσθεσα στο Inspector του Tilemap το Composite Collider 2D για να κάνω τα Colliders πιο εύκολα διαχειρίσιμα για τα γραφικά του παιχνιδιού. Για τα Collectibles όρισα στον κώδικα του ήρωα την ζωή του και έκανα αυτή την τιμή (μαζί με την ταχύτητα) να είναι επεξεργάσιμη από το Inspector του ήρωα. Κατέβασα ένα ακόμη Sprite Sheet για να βάλω ένα Collidable για την ζωή (trigger) του ήρωα και του πρόσθεσα στο Inspector το Box Collider 2D, έκανα check στο “is a trigger” και τέλος του άλλαξα το χρώμα. 

(Το sprite της ζωής)

(Το sprite sheet  για τα Health Collidables τα Damage Zones και το Projectile)

Δημιούργησα ένα καινούριο script για τα Health Colliders και το έβαλα στο triggers.
 Αφού έκανα public void της ζωής στον κώδικα του ήρωα έκανα prefab το collectable. Έβαλα 3 Damage Zones και έφτιαξα ένα καινούριο script για αυτά.

(Το Damage Zone)
Στην συνέχεια έβαλα στον κώδικα του ήρωα την εντολή Invincible Timer με τιμή 2.0f ούτως ώστε ο ήρωας όταν μένει στο Damage Zone να χάνει μία ζωή ανά δύο frames. Τέλος δημιούργησα και ένα prefab για το Damage Zone. Για τον εχθρό βρήκα ένα Sprite Sheet (το έκανα slice) και το έβαλα ώς trigger με BoxCollider2D και RigidBody2D και έφτιαξα ένα καινούριο script για αυτόν.

(Το sprite Sheet για τον εχθρό) 
 Τέλος έφτιαξα από τον κώδικα να κάνει Damage στον ήρωα κάθε φορά που αλληλεπιδρούν μεταξύ τους. Για το animation του εχθρού έφτιαξα ένα Animation Controller για αυτόν και έβαλα στο Inspector του το Animator. Δημιούργησα animations για τον εχθρό όταν κινείται πάνω κάτω δεξιά και αριστερά (χρισημοποιόντας και το FlipX απο τον editor του animation για να κινείται ο εχθρός από τις αντίθετες κατευθύνσεις με το ίδιο animation). Στο animator έφτιαξα ένα Blend Tree και αφού δημιούργησα δύο Float εντολές (Move X, Move Y)  έβαλα τις τέσσερις κατεύθυνσης κίνησης. Στον κώδικα του εχθρού όρισα αυτές τις Float εντολές και μετά έβαλα τον εχθρό να πηγαίνει μόνο παράλληλα με τον οριζόντιο άξονα. Στην συνέχεια, επειδή το sprite sheet που είχα για τον χαρακτήρα δεν είχε sprites που θα κινούταν ο ήρωας πάνω και κάτω, βρήκα ένα καινούριο sprite sheet και έφτιαξα όλες τις ρυθμίσεις του στο Inspector να είναι ίδιες με του προηγούμενου ήρωα (RigidBody2D, BoxCollider2D,...) και του έβαλα και το script που έχω για τον ήρωα.

(Ο καινούριος ήρωας)
 Με την ίδια διαδικασία που έφτιαξα το animation του εχθρού έφτιαξα περίπου και του ήρωα. Αρχικά έφτιαξα animations και για τις τέσσερις κινήσεις (πάνω, κάτω, δεξιά, αριστερά) αλλά και ένα animation (που δεν είναι πραγματικά animation γιατί έχει ένα frame) για μια κατάσταση Idle δηλαδή όταν ο ήρωας δεν θα έχει κανένα Input και θα είναι ακίνητος. Στο animator έφτιαξα ένα Blend Tree για τον παίκτη να κινείται στις τέσσερις κατευθύνσεις και έβαλα πάλι δύο καινούριες float εντολές (Look X, LookY, Speed). Στην συνέχεια έφτιαξα και ένα καινούριο animation για τον ήρωα όταν χτυπιέται και το έβαλα στο animator και δημιούργησα μία trigger εντολή ονομάζοντάς την Hit. 

(Το animator αρχικά) 
Για το Projectile βρήκα ένα sprite απο το spritesheet που είχα κατεβάσει για τα Health Collectables και τα Damage Zones και το πρόσθεσα στο Main Scene.

(Το projectile μου) 
Στο Inspector του έβαλα το RigidBody2D και το BoxCollider2D και έφτιαξα ένα καινούριο script στον φάκελο scripts όπου το ονόμασα Projectile. Έφτιαξα ένα καινούριο animation για να “πυροβολεί” ο ήρωας το projectile, το έβαλα στο animator και έφτιαξα τα transitions του (Όλα τα transitions δεν έχουν Exit Time και το Transitions Duration είναι 0).

(Το τελικό animator του ήρωα)

(Όλα τα animation του ήρωα)
 Έφτιαξα τα layers του ήρωα και του Projectile δημιουργώντας δύο καινούργια layers (Character, Projectile) και άλλαξα το layer στον Inspector από Default σε Character και Projectile αντίστοιχα. Μετά από τα project settings στα Physics 2D έκανα un-check τις αλληλεπιδράσεις μεταξύ του ήρωα και του projectile.

 Μετά έφτιαξα τον κώδικα του εχθρού και του projectile ούτως ώστε να αλληλεπιδρούν και τώρα ο εχθρός όταν “τρώει την σφαίρα”  σταματάει να κινείται και δεν μπορεί να κάνει damage στον ήρωα. Στην συνέχεια έφτιαξα ένα animation για τον εχθρό που θα μένει ακίνητος και θα κουνιέται όταν “τρώει την σφαίρα”.

(Το τελικό animator του εχθρού)

(Το τελικό Inspector του εχθρού)
 Για την camera κατέβασα το Cinemachine, έφτιαξα μια 2D camera και στο Inspector της έβαλα να ακολουθεί τον ήρωα. 
(Ο χάρτης με την κάμερα)

(Το Inspector της κάμερας)

Τέλος μεγάλωσα κι’ άλλο τον χάρτη (προσθέτοντας tiles νερού γύρω από τον ήδη υπάρχοντα) και έβαλα κι΄ άλλα damage zones καθώς και health collectables. 
(Ο τελικός χάρτης)


 (Το Hierarchy μου)

(Όλα τα prefabs) 

(Όλα τα scripts)

(Το τελικό Inspector του ήρωα)

ΠΡΟΒΛΗΜΑΤΑ: 1) Όταν το animation είναι σε κάποια άλλη κατάσταση εκτός από το Blend Tree (Hit, Shoot) πρέπει να αλληλεπιδράσει δύο φορές για να γυρίσει στην κατάσταση της κίνησης (Blend Tree ή Idle). 
ΠΡΟΤΆΣΕΙΣ ΒΕΛΤΊΩΣΗΣ: 
1) Να φτιάξω καλύτερο χάρτη 
2) Να φτιάξω καλύτερα animation για το Hit και το Shoot (και μάλλον να αλλάξω χαρακτήρα καθώς ήταν πολύ φτωχός στο πλήθος τον διαφορετικών sprites) 


# 3rd Deliverable 


# Conclusions


# Sources
