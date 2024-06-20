# Παιχνίδι Κρεμάλα

Αυτό το παιχνίδι της κρεμάλας επιτρέπει στους παίκτες να μαντέψουν λέξεις επιλέγοντας γράμματα από το ελληνικό αλφάβητο. Ο κώδικας χρησιμοποιεί session για την αποθήκευση της τρέχουσας κατάστασης του παιχνιδιού, όπως η λέξη που πρέπει να μαντευτεί και τα γράμματα που έχουν ήδη μαντευτεί.

## Αρχικοποίηση Λιστών

- **Λίστα Γραμμάτων (`$letters`):** Περιέχει όλα τα γράμματα του ελληνικού αλφαβήτου.
- **Λίστα Λέξεων (`$words`):** Περιέχει τις λέξεις που πρέπει να μαντέψει ο παίκτης.

## Επιλογή Τυχαίας Λέξης και Αρχικοποίηση Session

- Εάν δεν έχει ήδη επιλεχθεί μια λέξη (δηλαδή, αν δεν υπάρχει λέξη στο session), επιλέγεται τυχαία μια λέξη από τη λίστα `$words` και αποθηκεύεται στο session.
- Το session αρχικοποιείται επίσης για να αποθηκεύει τα γράμματα που έχουν μαντευτεί από τον παίκτη.

## Διαχείριση Υποβολής Γραμμάτων

- Όταν ο παίκτης υποβάλει ένα γράμμα μέσω της φόρμας, το γράμμα προστίθεται στη λίστα των μαντεμένων γραμμάτων εάν δεν έχει ήδη μαντευτεί.
- Η λίστα των μαντεμένων γραμμάτων αποθηκεύεται στο session.

## Εμφάνιση της Λέξης και των Κουμπιών Γραμμάτων

- Η λέξη εμφανίζεται με τα μαντεμένα γράμματα στη θέση τους και κάτω παύλες (`_`) για τα υπόλοιπα γράμματα.
- Τα κουμπιά των γραμμάτων εμφανίζονται δυναμικά. Εάν ένα γράμμα έχει ήδη μαντευτεί, το κουμπί του γράμματος απενεργοποιείται.

