# Δημιουργία εύκολων προσβάσιμων ιστοσελίδων

![All About Accessibility](webdev101-a11y.png)
> Sketchnote by [Tomomi Imura](https://twitter.com/girlie_mac)

## Pre-Lecture Quiz
[Pre-lecture quiz](https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/5)

> Η δύναμη του Ιστού βρίσκεται στην καθολικότητά του. Η πρόσβαση από όλους ανεξαρτήτως αναπηρίας αποτελεί βασική αρχή.
>
> \- Sir Timothy Berners-Lee, W3C Director and inventor of the World Wide Web

Το απόσπασμα αυτό επισημαίνει τέλεια τη σημαντικότητα του να δημιουργείς εύκολα προσβάσιμες ιστοσελίδες. Μια εφαρμογή στην οποία δεν είναι δυνατή η πρόσβαση από όλους είναι εξ ορισμού αποκλειστική. Ως web developers πρέπει πάντα να έχουμε κατά νου την προσβασιμότητα. Έχοντας αυτό στο μυαλό σας από την αρχή, θα βρίσκεστε σε καλό δρόμο για να διασφαλίσετε ότι όλοι θα έχουν πρόσβαση στις σελίδες που δημιουργείτε. Σε αυτό το μάθημα, θα μάθετε για τα εργαλεία που μπορούν να σας βοηθήσουν να διασφαλίσετε ότι τα στοιχεία στο web σας θα είναι εύκολα προσβάσιμα και πώς μπορείτε εσείς να θα φτιάξετε κάτι τέτοιο.

## Εργαλεία

### Screen readers

Ένα από τα πιο γνωστά εργαλεία προσβασιμότητας είναι οι screen readers.

Οι [Screen readers](https://en.wikipedia.org/wiki/Screen_reader) είναι clients που χρησιμοποιούνται συνήθως για άτομα με προβλήματα όρασης. Όπως ξοδεύουμε χρόνο στο να διασφαλίσουμε ότι ένας browser μεταφέρει σωστά τις πληροφορίες που θέλουμε να μοιραστούμε, πρέπει αντίστοιχα να διασφαλίσουμε ότι ο screen reader θα κάνει το ίδιο.

Στη πιο βασική του χρήση, ένας screen reader διαβάζει μια σελίδα από πάνω προς τα κάτω. Εάν η σελίδα σας αποτελείται εξ ολοκλήρου από κείμενο, ο reader θα διαβάσει τις πληροφορίες με παρόμοιο τρόπο όπως σε ένα ήταν σε ένα browser. Φυσικά, οι ιστοσελίδες είναι σπάνια καθαρά κείμενο. Θα περιέχουν συνδέσμους, γραφικά, χρώμα και άλλα οπτικά στοιχεία. Πρέπει να ληφθεί μέριμνα ώστε οι πληροφορίες αυτές να διαβαστούν σωστά από έναν screen reader.

Κάθε web developer πρέπει να εξοικειωθεί με τον screen reader. Όπως τονίστηκε παραπάνω, είναι ο client που θα χρησιμοποιήσουν οι χρήστες σας. Όπως είστε εξοικειωμένοι με τον τρόπο λειτουργίας ενός browser, έτσι θα πρέπει να εξοικειωθείτε και να μάθετε πώς λειτουργεί ένας screen reader. Ευτυχώς, οι screen readers είναι ενσωματωμένοι στα περισσότερα λειτουργικά συστήματα.

Ορισμένοι browser διαθέτουν επίσης ενσωματωμένα εργαλεία και extensions που μπορούν να διαβάζουν κείμενο ή ακόμη και να παρέχουν ορισμένες βασικές λειτουργίες πλοήγησης, όπως [these accessibility-focused Edge browser tools](https://support.microsoft.com/en-us/help/4000734/microsoft-edge-accessibility-features). Αυτά είναι επίσης σημαντικά εργαλεία προσβασιμότητας, αλλά λειτουργούν πολύ διαφορετικά από τους screen readers και δεν θα πρέπει να ταυτίζονται με τους screen readers.

✅ Δοκιμάστε έναν screen reader και ένα browser text reader. Στα Windows [Narrator](https://support.microsoft.com/en-us/windows/complete-guide-to-narrator-e4397a0d-ef4f-b386-d8ae-c172f109bdb1) περιλαμβάνεται by default και επίσης [JAWS](https://webaim.org/articles/jaws/) και [NVDA](https://www.nvaccess.org/about-nvda/) μπορεί να εγκατασταθεί. Σε macOS και iOS, το [VoiceOver] (https://support.apple.com/guide/voiceover/welcome/10) είναι εγκατεστημένο by default.

### Zoom

Ένα άλλο εργαλείο που χρησιμοποιείται συνήθως από άτομα με προβλήματα όρασης είναι το zoom. Ο πιο βασικός τύπος zoom είναι το στατικό zoom, που ελέγχεται μέσω του «Control + σύμβολο πρόσθεσης (+)» ή μειώνοντας την ανάλυση της οθόνης. Αυτός ο τύπος zoom προκαλεί αλλαγή μεγέθους ολόκληρης της σελίδας, επομένως η χρήση του [responsive design] (https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design) είναι σημαντική για την παροχή μιας καλής εμπειρίας χρήστη σε αυξημένα επίπεδα zoom.

Ένας άλλος τύπος zoom βασίζεται σε εξειδικευμένο λογισμικό το οποίο μεγεθύνει μία μόνο περιοχή της οθόνης και μπορείτε να μετακινήσετε αυτή τη μεγέθυνση, σαν να χρησιμοποιούσατε έναν πραγματικοό μεγεθυντικό φακό. Στα Windows, το [Magnifier] (https://support.microsoft.com/en-us/windows/use-magnifier-to-make-things-on-the-screen-easier-to-see-414948ba-8b1c-d3bd -8615-0e5e32204198) είναι ενσωματωμένο και το [ZoomText] (https://www.freedomscientific.com/training/zoomtext/getting-started/) είναι ένα third-party λογισμικό μεγέθυνσης με περισσότερες δυνατότητες και μεγαλύτερη βάση χρηστών. Τόσο το macOS όσο και το iOS διαθέτουν ένα ενσωματωμένο λογισμικό μεγέθυνσης που ονομάζεται [Zoom] (https://www.apple.com/accessibility/mac/vision/). 

### Contrast checkers

Τα χρώματα στα web sites πρέπει να επιλέγονται προσεκτικά για να ανταποκρίνονται στις ανάγκες των χρηστών με αχρωματοψία ή άτομα που δυσκολεύονται να δουν χρώματα χαμηλής αντίθεσης.

✅ Τεστάρετε τη χρήση χρώματος ενός web site που σας αρέσει χρησιμοποιώντας ένα browser extension όπως το [WCAG's color checker](https://microsoftedge.microsoft.com/addons/detail/wcag-color-contrast-check/idahaggnlnekelhgplklhfpchbfdmkjp?hl=en-US). Τι μάθατε;

### Lighthouse

Στην περιοχή στην οποία βρίσκονται τα developer tools στον browser σας, θα βρείτε το Lighthouse tool. Αυτό το εργαλείο είναι σημαντικό για να έχετε μία πρώτη ιδέα για την προσβασιμότητα(αλλά και για άλλες αναλύσεις) ενός web site. Παρόλο που καλό θα ήταν να μη βασίζεστε αποκλειστικά και μόνο στο Lighthouse, η βαθμολογία 100% που έχει δείχνει ότι είναι πολύ καλό για να το χρησιμοποιήσετε έστω και σαν βάση.

✅ Βρείτε το Lighthouse στο developer tool panel στον browser σας και τρέξτε μία ανάλυση σε κάποιο site. Τι παρατηρείτε;

## Σχεδιασμός για προσβασημότητα

Η προσβασιμότητα είναι ένα σχετικά ευρύ θέμα. Για να σας βοηθήσουμε, υπάρχουν αρκετές πηγές διαθέσιμες.

- [Accessible U - University of Minnesota](https://accessibility.umn.edu/your-role/web-developers)

Ενώ δεν θα μπορέσουμε να καλύψουμε κάθε πτυχή της δημιουργίας προσβάσιμων site, παρακάτω βρίσκονται μερικές βασικές αρχές που θα θέλατε να εφαρμόσετε. Η σχεδίαση μίας προσβάσιμης σελίδας από την αρχή είναι **πάντα** ευκολότερη από το να πηγαίνετε σε μία ήδη υπάρχουσα σελίδα και να προσπαθείτε να την κάνετε προσβάσιμη.

## Good display principles

### Color safe palettes

Οι άνθρωποι βλέπουν τον κόσμο με διαφορετικό τρόπο. Το ίδιο συμβαίνει και με τα χρώματα. Κατά την επιλογή των χρωμάτων για το site σας, πρέπει να διασφαλίσετε ότι είναι προσβάσιμο σε όλους. Ένα πολύ καλό εργαλείο [tool for generating color palettes is Color Safe](http://colorsafe.co/).

✅ Εντοπίστε ένα site το οποίο είναι πολύ προβληματικό όσον αφορά τα χρώματά του. Γιατί το διαλέξατε;

### Χρησιμοποιείστε τη σωστή HTML

Με τη CSS και τη Javascript μπορείτε να κάνετε οποιοδήποτε element να φαίνεται σαν οποιοδήποτε τύπο control. Το `<span>` μπορεί να χρησιμοποιηθεί για τη δημιουργία ενός `<button>` και το `<b>` μπορεί να γίνει ένας υπερσύνδεσμος(hyperlink). Παρόλο που αυτό μπορεί να θεωρηθεί ευκολότερο στο να κατασκευαστεί, δεν μπορεί να αναγνωριστεί από τους screen readers. Χρησιμοποιήστε την κατάλληλη HTML όταν δημιουργείτε controls σε μία σελίδα. Αν θέλετε να χρησιμοποιήσετε ένα hyperlink, χρησιμοποιήστε `<a>`. Η χρησιμοποίηση της σωστής HTML για το σωστό control αποτελεί το σημασιολογικό της HTML.

✅ Πηγαίνετε σε οποιοδήποτε site και δείτε αν οι designers και οι developers χρησιμοποιούν σωστά την HTML. Μπορείτε να βρείτε ένα κουμπί το οποίο θα έπρεπε κανονικά να είναι link; Hint: κάντε δεξί κλικ και επιλέξτε 'View Page Source' στον browser για να δείτε τον κώδικα που βρίσκεται από πίσω.

### Δημιουργήστε μία περιγραφικη επικεφαλίδα

Οι χρήστες των screen readers [βασίζονται πολύ στις επικεφαλίδες](https://webaim.org/projects/screenreadersurvey8/#finding) για να βρουν πληροφορίες και να περιηγηθούν σε μία σελίδα. Η συγγραφή περιγραφικών επικεφαλίδων και η χρησιμοποίηση των σημασιολογικών heading tags είναι σημαντικά για τη δημιουργία μίας εύκολα περιηγήσιμης σελίδας από άτομα που χρησιμοποιούν screen readers.

### Χρησιμοποιήστε καλές οπτικές ενδείξεις

Η CSS προσφέρει πλήρη έλεγχο επάνω στην εμφάνιση οποιουδήποτε στοιχείου σε μία σελίδα. Μπορείτε να δημιουργήσετε πλαίσια κειμένου(text boxes) χωρίς περίγραμμα(outline) και υπερσυνδέσμους(hyperlinks) χωρίς υπογράμμιση(underline). Δυστυχώς η αφαίρεση αυτών των στοιχείών μπορεί να κάνει την περιήγηση πιο δύσκολη σε κάποιον ο οποίος εξαρτάται από αυτά τα χαρακτηριστικά για να αναγνωρίσει το είδος του control.

## Η σημαντικότητατου link text

Οι υπερσύνδεσμοι αποτελόυν τη βάση για την περιήγηση στο διαδίκτυο. Ως αποτέλεσμα, η διασφάλιση ότι ένας screen reader μπορεί να διαβάσει σωστά τα links επιτρέπει σε όλους τους χρήστες να περιηγηθούν στο site.

### Screen readers και links

Όπως θα περιμένατε, οι screen readers διαβάζουν τα links με τον ίδιο τρόπο που θα διάβαζαν οποιοδήποτε άλλο κείμενο στη σελίδα. Έχοντας αυτό στο μυαλό, το κείμενο που παρουσιάζεται παρακάτω μπορεί να είναι απολύτως αποδεκτό.

> The little penguin, sometimes known as the fairy penguin, is the smallest penguin in the world. [Click here](https://en.wikipedia.org/wiki/Little_penguin) for more information.

> The little penguin, sometimes known as the fairy penguin, is the smallest penguin in the world. Visit https://en.wikipedia.org/wiki/Little_penguin for more information.

> **ΣΗΜΕΙΩΣΗ** Όπως θα δείτε παρακάτω, δεν πρέπει **ποτέ** να φτιάχνετε links που μοιάζουν με τα παραπάνω.

Θυμηθείτε, οι screen readers είναι διαφορετικό interface από τους browsers και έχουν διαφορετικό σύνολο χαρακτηριστικών.

### Το πρόβλημα με τo URL

Οι screen readers διαβάζουν κείμενο. Αν ένα URL εμφανιστεί, ο screen reader θα διαβάσει το URL. Γενικά μιλώντας, το URL δεν μεταφέρει σηματικές πληροφορίες και ακούγεται ενοχλητικό. Ίσως να έχει τύχει να το ακούσετε αν το τηλέφωνό σας έχει διαβάσει ποτέ δυνατά ένα μήνυμα που περιέχει URL.

### Το πρόβλημα με το "click here"

Οι screen readers έχουν επίσης τη δυνατότητα να διαβάζουν μόνο τa hyperlinks σε μία σελίδα, με τον ίδιο τρόπο με τον οποίο ένα άτομο που διαθέτει όραση θα σκάναρε τη σελίδα για links. Αν  όλα τα links του κειμένου είναι του τύπου "click here", το μόνο που θα ακούσουν οι χρήστες είναι "click here, click here, click here, click here, click here, ..." Όλα τα links είναι πλέον αδιάκριτοι μεταξύ τους.

### Καλό link text

Ένα καλό link text περιγράφει εν ολίγης τι βρίσκεται στην άλλη μερία του link. Στο παραπάνω παράδειγμα με τους μικρούς πιγκουίνους, το link είναι από τη σελίδα Wikipedia σχετικά με το είδος των πιγκουίνων. Η φράση *little penguins* θα ήταν το τέλειο link text διότι κάνει ξεκάθαρο το τι πρόκειται να μάθει κάποιος αν πατήσει το link - μικρούς πιγκουίνους.

> Οι [μικροί πιγκουίνοι](https://en.wikipedia.org/wiki/Little_penguin), γνωστοί και ως πιγκουίνοι νεράιδες, είναι οι μικρότεροι πιγκουίνοι στον κόσμο.

✅ Περιηγηθείτε για μερικά λεπτά στο διαδίκτυο για να βρείτε σελίδες που χρησιμοποιούν δυσνόητα link. Συγκρίνετέ τα με links από άλλα sites που χρησιμοποιούν καλύτερα ονόματα για links τους. Τι μάθατε;

#### Σημειώσεις μηχανής αναζήτησης

Σαν επιπλέον διασφάλιση ότι το site είναι προσβάσιμο σε όλους, θα πρέπει να βοηθήσετε και τις μηχανές αναζήτησης να περιηγηθούν μέσα σε αυτό. Οι μηχανές αναζήτησης χρησιμοποιούν link text για να μάθουν τα θέματα τις σελίδας. Οπότε το να χρησιμοποιήσετε καλό link text θα τους βοηθήσει όλους!

### ARIA

Φανταστείτε την ακόλουθη σελίδα:

| Product      | Description        | Order        |
| ------------ | ------------------ | ------------ |
| Widget       | [Description]('#') | [Order]('#') |
| Super widget | [Description]('#') | [Order]('#') |

Σε αυτό το παράδειγμα, το να επαναλάβετε το περιεχόμενο του description και του order βγάζει νόημα για κάποιον που χρησιμοποιεί browser. Ωστόσο, κάποιος που χρησιμοποιεί screen reader θα άκουγε μόνο τις λέξεις *description* και *order* να επαναλαμβανονται χώρις κάποια επιπλέον πληροφορία.

Για την υποστήριξη τέτοιων σεναρίων, η HTML υποστηρίζει ένα σύνολο από χαρακτηριστικών γνωστά ως [Accessible Rich Internet Applications (ARIA)](https://developer.mozilla.org/docs/Web/Accessibility/ARIA). Τα χαρακτηριστικά αυτά σας επιτρέπουν να προμηθεύσετε τους screen readers με επιπλέον πληροφορία.

> **ΣΗΜΕΙΩΣΗ**: Όπως πολλές πτυχές της HTML, έτσι και η υποστήριξη browser και screen reader μπορεί να διαφέρει. Ωστόσο, οι περισσότεροι βασικοί clients υποστηρίζουν ARIA χαρακτηριστικά.

Μπορείτε να χρησιμοποιήσετε `aria-label` για να περιγράψετε το link όταν η μορφή της σελίδας δεν σας το επιτρέπει. Η περιγραφή για το widget θα μπορούσε να οριστεί ως

``` html
<a href="#" aria-label="Widget description">description</a>
```

✅ Γενικά, η χρήση σημασιολογίας σήμανσης όπως περιγράφεται παραπάνω αντικαθιστά τη χρήση του ARIA, άλλα μερικές φορές δεν υπάρχει ισοδύναμη σημασιολογία για διάφορα HTML widgets. Ένα καλό παράδειγμα είναι ένα Δέντρο. Δεν υπάρχει ισοδύναμη HTML για ένα δέντρο, οπότε χρησιμοπποιείται το γενικό `<div>` για αυτή τη δουλειά με τις κατάλληλες aria τιμές. Το [MDN documentation on ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) περιέχει μερικές χρήσιμες πληροφορίες.

```html
<h2 id="tree-label">File Viewer</h2>
<div role="tree" aria-labelledby="tree-label">
  <div role="treeitem" aria-expanded="false" tabindex="0">Uploads</div>
</div>
```

## Εικόνες

Είναι αυτονόητο ότι οι screen readers δεν μπορούν να διαβάσουν αυτόματα μία εικόνα και οτιδήποτε βρίσκεται μέσα σε αυτή. Για να κάνετε τις εικόνες προσβάσιμες δεν απαιτείται ιδιαίτερος κόπος - όλη η ουσία βρίσκεται στο `alt`. Όλες οι εικόνες που φέρουν κάποιο μήνυμα θα πρέπει να έχουν ένα `alt` για να περιγράφει το τι είναι.
Οι εικόνες που είναι καθαρά διακοσμητικές και δεν έχουν κάποιο νόημα-κείμενο στο εσωτερικό τους θα πρέπει να ορίσουν το `alt` τους με μία κενή συμβολοσειρά: `alt=""`. Αυτό αποτρέπει τους screen readers από το να διαβάσουν αχρείαστες διακοσμητικές εικόνες.

✅ Όπως ίσως περιμένατε, και οι μηχανές αναζήτησης δεν μπορούν να καταλάβουν το περιεχόμενο μίας εικόνας. Χρησιμοποιούν και αυτές το alt. Οπότε για μία ακόμη φορά, η διασφάλιση ότι η σελίδα σας είναι προσβάσιμη παρέχει επιπλέον μπόνους!

## Το πληκτρολόγιο

Κάποιοι χρήστες δεν μπορούν να χρησιμοποιήσουν ποντίκι ή trackpad και αντ' αυτού στηρίζονται μόνο στο πληκτρολογιο για να μετακινηθούν από ένα στοιχείο της σελίδας σε ένα άλλο. Είναι σημαντικό για τη σελίδα σας να παρουσιάζει το περιοχόμενό της σε λογική σειρά ώστε κάποιο χρήστης που χρησιμοποιεί μόνο το πληκτρολόγιο να μπορεί να αλληλεπιδρά με το κάθε στοιχείο καθώς κάνει scroll σε ένα αρχείο. Αν φτιάξετε τις σελίδες σας με σημασιολογική σήμανση(semantic markup) και χρησιμοποιήσετε CSS για να τη διακοσμήσετε, η σελίδα σας λογικά θα είναι πλοηγήσιμη από το πληκτρολόγιο, αλλά είναι σημαντικό να το τεστάρετε οι ίδιοι. Μάθετε περισσότερα για [keyboard navigation strategies](https://webaim.org/techniques/keyboard/).

✅ Πηγαίνετε σε κάποιο site και προσπαθήστε να περιηγηθείτε χρησιμοποιώντας μόνο το πληκτρολόγιο. Τι λειτουργεί, τι δεν λειτουργεί και γιατί;

## Σύνοψη

Ένας ιστός προσβάσιμος σε μερικούς δεν είναι πραγματικά ένας 'παγκοσμίου εμβέλιας ιστός'. Ο καλύτερος τρόπος για να διασφαλίσετε ότι οι σελίδες που δημιουργείτε είναι προσβάσιμες είναι να ενσωματώσετε τις καλύτερες πρακτικές προσβασιμότητας από την αρχή. Παρόλο που περιλαμβάνει επιπλέον κόπο, η ενσωμάτωση αυτών των τεχνικών στη δουλεία σας θα σημαίνει ότι όλες οι σελίδες που δημιουργείτε θα είναι προσβάσιμες.

---

## 🚀 Challenge

Πάρτε αυτήν την HTML και ξαναγράψτε την έτσι ώστε να είναι όσο περισσότερο προσβάσιμη γίνεται, χρησιμοποιώντας τις τεχνικές που μάθατε.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>
      Example
    </title>
    <link href='../assets/style.css' rel='stylesheet' type='text/css'>
  </head>
  <body>
    <div class="site-header">
      <p class="site-title">Turtle Ipsum</p>
      <p class="site-subtitle">The World's Premier Turtle Fan Club</p>
    </div>
    <div class="main-nav">
      <p class="nav-header">Resources</p>
      <div class="nav-list">
        <p class="nav-item nav-item-bull"><a href="https://www.youtube.com/watch?v=CMNry4PE93Y">"I like turtles"</a></p>
        <p class="nav-item nav-item-bull"><a href="https://en.wikipedia.org/wiki/Turtle">Basic Turtle Info</a></p>
        <p class="nav-item nav-item-bull"><a href="https://en.wikipedia.org/wiki/Turtles_(chocolate)">Chocolate Turtles</a></p>
      </div>
    </div>
    <div class="main-content">
      <div>
        <p class="page-title">Welcome to Turtle Ipsum. 
            <a href="">Click here</a> to learn more.
        </p>
        <p class="article-text">
          Turtle ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum
        </p>
      </div>
    </div>
    <div class="footer">
      <div class="footer-section">
        <span class="button">Sign up for turtle news</span>
      </div><div class="footer-section">
        <p class="nav-header footer-title">
          Internal Pages
        </p>
        <div class="nav-list">
          <p class="nav-item nav-item-bull"><a href="../">Index</a></p>
          <p class="nav-item nav-item-bull"><a href="../semantic">Semantic Example</a></p>
        </div>
      </div>
      <p class="footer-copyright">&copy; 2016 Instrument</span>
    </div>
  </body>
</html>
```

## Post-Lecture Quiz
[Post-lecture quiz](https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/6)

## Review & Self Study

Πολλές κυβερνήσεις έχουν νόμους σχετικά με τις απαιτήσεις για την προσβασιμότητα. Διαβάστε τους νόμους της χώρας σας για τις απαιτήσεις για την προσβασιμότητα. Τι περιλαμβάνει και τι δεν περιλαμβάνει; Ένα παράδειγμα είναι το [this government web site](https://accessibility.blog.gov.uk/).

## Assignment
 
[Αναλύστε μία μη προσβάσιμη σελίδα](assignment.md)

Credits: [Turtle Ipsum](https://github.com/Instrument/semantic-html-sample) by Instrument

