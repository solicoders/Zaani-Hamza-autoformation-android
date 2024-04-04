---
layout: default
chapitre: Présentation de Kotlin
order: 2
---

# Présentation de Kotlin

```kotlin
fun main() {
    println("Hello, world!")
}
```
```kotlin
Hello, world!
```
<!-- new slide -->

## Examples

```kotlin
fun main() {
    val count : Int = 2
    println(count)
}
```
```kotlin

fun main() {
    val count: Int = 2
    println("You have $count unread messages.")
}

```
```kotlin
fun main() {
    birthdayGreeting()
    println(birthdayGreeting())
}
```
```kotlin
fun birthdayGreeting(): String {
    val nameGreeting = "Happy Birthday, Rover!"
    val ageGreeting = "You are now 5 years old!"
    return "$nameGreeting\n$ageGreeting"
}
```
```kotlin
fun main() {
    birthdayGreeting()
}
```
```kotlin
fun birthdayGreeting(): Unit {
    println("Happy Birthday, Rover!")
    println("You are now 5 years old!")
}
```
```kotlin
fun main() {
    birthdayGreeting("Ahmed")
    println(birthdayGreeting("Ahmed"))
}
```
```kotlin
fun birthdayGreeting(name: String): String {
    val nameGreeting = "Happy Birthday, $name!"
    val ageGreeting = "You are now 5 years old!"
    return "$nameGreeting\n$ageGreeting"
}
```
```kotlin
fun main() {
    birthdayGreeting("Ahmed",24)
    println(birthdayGreeting("Ahmed",24))
}
```
```kotlin
fun birthdayGreeting(name: String, age: Int): String {
    val nameGreeting = "Happy Birthday, $name!"
    val ageGreeting = "You are now $age years old!"
    return "$nameGreeting\n$ageGreeting"
}
```
## exercice 1 
### Passage par valeur 
```kotlin 
fun main() {
    var nom = "Fouad"
    var bonjour_nom = Bonjour(nom)
    println (bonjour_nom)
    println (nom)
}

fun Bonjour(nom:String):String{
    nom =  "Bonjour" + nom
    return nom
}
```
- Donnez le nombre d'instructions 
- Donnez le nombre de variables utilisé dans le mémoire 


## Réponse 
```kotlin
fun main() {
  var nom = "Fouad"
  var bonjour_nom = Bonjour(nom)
  println (bonjour_nom)
  println (nom)
 }

fun Bonjour(nom:String):String{
  var nom =  "Bonjour" + nom
  return nom
}
```
### le nombre d'instructions 
  - 6 
### Donnez le nombre de variables utilisé dans le mémoire
  - 3


## TP - Fonctions
- Créer un programme qui demande deux valeurs à l'utilisateur. Ensuite, il calcule la somme de ces deux valeurs
## solution 
```kotlin 
fun main() {
    println("Entrez la première valeur :")
    val valeur1 = readLine()?.toDoubleOrNull()
    if (valeur1 == null) {
        println("Entrée invalide pour la première valeur.")
        return
    }

    println("Entrez la deuxième valeur :")
    val valeur2 = readLine()?.toDoubleOrNull()
    if (valeur2 == null) {
        println("Entrée invalide pour la deuxième valeur.")
        return
    }

    val somme = valeur1 + valeur2
    println("La somme de $valeur1 et $valeur2 est : $somme")
}


```