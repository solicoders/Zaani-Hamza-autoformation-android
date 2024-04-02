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
