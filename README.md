# remote-carbage-collecting-robot
Αποθετήριο του σχολείου "Εσπερινό ΕΠΑΛ Αλιάρτου" για στην συμμετοχή στον Διαγωνισμό Ανοιχτών Τεχνολογιών

**Ομάδα:  "Από μακριά και με Ασφάλεια"**(Οι μαθητές της **Β πληροφορικής** του Εσπερινού ΕΠΑΛ Αλιάρτου 

**Σχολείο:** Εσπερινό ΕΠΑΛ Αλιάρτου

**Τίτλος έργου:** «Σύστημα απομακρυσμένης συλλογής και διαλογής επικίνδυνων απορριμμάτων»

______

# Εποπτικό Διάγραμμα του Συστήματος

___

![Εποπτικό Διαγραμμα του Συστήματος](images/ELLAK-2-remote-carbage-colecting-robot-BLOCK-diagram-1.jpg)

______

# ΑΡΧΙΚΗ ΠΡΟΤΑΣΗ ΤΟΥ ΕΡΓΟΥ

___

Παρακάτω περιγράφεται η πρόταση έργου για την συμμετοχή της ομάδας μας ,**" Από μακριά και με Ασφάλεια "**, στον «4ο Πανελλήνιο Διαγωνισμό Ανοιχτών Τεχνολογιών στην Εκπαίδευση»

## Εισαγωγή - Περιγραφή

Στην παρούσα πρόταση, η ομάδα μας προτείνει την κατασκευή ενός συστήματος, που σκοπός του είναι να εκτελεί απομακρυσμένη συλλογή και διαλογή επικίνδυνων απορριμμάτων.

Πιο συγκεκριμένα, το παραπάνω σύστημα,  είναι σχεδιασμένο έτσι ώστε  να εκτελεί ενέργειες,  οι οποίες είναι δύσκολες ή επικίνδυνες για τον άνθρωπο ,  σχετικά με την συλλογή  ή  διαλογή   επικίνδυνο ή γενικότερα δύσχρηστων  απορριμμάτων.

Καρδιά του συστήματος αυτού,   είναι ένας **ρομποτικός βραχίονας**,  ο οποίος εκπαιδεύεται να κάνει συγκεκριμένες κινήσεις συλλέγοντας και τοποθετώντας στα κατάλληλα μέρη για ανακύκλωση ή  απόσυρση   των επικίνδυνων αυτών απορριμμάτων.  Ο βραχίονας αυτός κάνει τις κινήσεις  με τη βοήθεια  **σέρβοκινητήρων** ,  οι οποίοι ελέγχονται από ένα Arduino. Ο έλεγχος της παραπάνω ρομποτικής συσκευής γίνεται είτε με **κατάλληλο χειριστήριο** που θα κατασκευαστεί , καθώς επίσης και μέσω κινητού τηλεφώνου και **εφαρμογής για Android**  κινητά ή ταμπλέτες.  

Ένας **τοπικός ελεγκτής (Raspberry Pi Zero)**  είναι υπεύθυνος τόσο για την τοπική αποθήκευση των "συνταγών κινήσεων" κατά την διάρκεια της εκπαίδευσης  όσο και για την εκτέλεση τους όταν λάβει την κατάλληλη εντολή. Το σύστημα που προτείνουμε αποτελείται από ένα ρομποτικό βραχίονα αλλά σε μία πλήρη ανάπτυξη η γραμμή παραγωγής θα αποτελούνταν από πολλούς τέτοιους ρομποτικούς βραχίονες. 

Για το συντονισμό και ελέγχου όλης αυτής της αυτοματοποιημένης γραμμής συλλογής απορριμμάτων, είναι απαραίτητος ο  **τοπικός σταθμός ελέγχου (Raspberry Pi 4)** .  Εκτός από τον προαναφερόμενο συντονισμό ο σταθμός αυτός είναι επιφορτισμένος και με  με το επικοινωνιακό έργο προς τον έξω κόσμο. Με άλλα λόγια ο σταθμός αυτούς Μπορεί να συνδεθεί στο διαδίκτυο internet και μέσα από εκεί να πάρει τις κατάλληλες εντολές για να εκτελέσει το έργο του.

Μέσα από την παραπάνω  δομή επιτυγχάνουμε το control room , **ο κεντρικός σταθμός ελέγχου**  να βρίσκεται οπουδήποτε στον κόσμο  σε ασφαλές περιβάλλον και μέσω αυτού  να μπορούμε να προγραμματίζουμε , να εποπτεύουμε  και να εκτελούμε όλες τις δύσκολες και επικίνδυνες ενέργειες  για την συλλογή επικίνδυνων ρύπων


# Τι παρόμοιο υπάρχει - Τρέχουσα αντιμετώπιση προβλήματος

Στην προσπάθειά μας να ερευνήσουμε την τρέχουσα κατάσταση και να παρατηρήσουμε τι λύσεις υπάρχουν σε παρόμοια προβλήματα καταλήξαμε στις παρακάτω διαπιστώσεις:

-  Υπάρχουν αρκετές συσκευές αυτοματοποίησης στον χώρο της συγκομιδής και διαλογής  απορριμμάτων,  όμως αυτές είναι προσανατολισμένες σε  **κεντρικοποιημένες  δομές μεγάλου κόστους** οι οποίες βασίζονται στην στη  **μεταφορά** από τους χώρους παραγωγής των απορριμμάτων στον κεντρικό σταθμό

-   το σύστημά μας μειώνει τις μεταφορές προτείνοντας την επιτόπου διαχείριση (κατά συνέπεια  **εξοικονόμηση πόρων** , καυσίμων και μείωση εκπομπών διοξειδίου του άνθρακα)

-    επενδύει στην  **εξ αποστάσεως εργασία**,  η οποία στις μέρες μας  γίνεται όλο και πιο ελκτική έως και απαραίτητη

-    θέτει σε πρώτο πλάνο την  **ασφάλεια του ανθρώπου  στο περιβάλλον εργασίας**

-    στηρίζεται σε  **ανοιχτές τεχνολογίες**  προσπαθώντας να αντικαταστήσει κλειστές και πολύ ακριβές κατασκευές

-    λόγω των ανοιχτών τεχνολογιών είναι  **εύκολα επεκτάσιμο και εξελίξιμο**
