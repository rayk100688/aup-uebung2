# aup-uebung2
tasks for learning the language "Rust"

Aufgabe1

Erstelle eine rekursive Funktion is_multiple(larger:f32,smaller:f32)->bool, welche vergleicht ob larger ein vielfaches von smaller ist. Worauf muss man beim Vergleich von Gleitkommazahlen achten?

Aufgabe2

Implementieren Sie eine Funktion print_type welche den Typ der Eingabe in Textform auf der Konsole zurück gibt. Nur primitive Typen werden eingegeben. Welches Konzept der Vorlesung wird benötigt?

Aufgabe3

Implementieren Sie eine Funktion is_large welche für einen Wert eines beliebigen primitiven Zahlentyps zurückgibt ob der Wert bezogen auf den Wertebereich klein (untere Hälfte des Wertebereichs --> BOOL false) oder groß (Hälfte und größer im Wertebereich --> BOOL true) ist.

Aufgabe4

Implementieren Sie den Trait für f64 und u64:

trait Power {
  fn power(self, exp:u32)->Self;
}

Aufgabe5

Implementieren Sie den Trait für f64(Nachkommastellen auf 10000-stel runden) und u64:

trait DigitCounter {
  fn count_digits(self)->usize;
}

Die Funktion soll die Ziffern zählen

Aufgabe6

Gegeben ist dieser Trait:
trait CryptoMessage {
fn encrypt(self,key:u8)->Self;
fn decrypt(self,key:u8)->Self;
fn print_bytes(self);
}

Hier soll die Caesar-Chiffre angewendet werden.
Die Nachricht erfolgt in der Implementierung und soll byte-weise Modulo-Aufaddiert werden.
