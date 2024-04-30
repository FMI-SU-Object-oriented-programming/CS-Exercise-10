# Задача "Фентъзи свят"

Напишете абстрактен клас "Creature" който да има чист виртуален метод ``print()`` и низ (``char*``) за име

Напишете клас "Dragon", който наследява Creature и има метод ``breatheFire()``, който да отпечатва на екрана "RRAAGGHHH!!!"

Напишете клас "Wizard", който наследява Creature и има метод ``castMagic()``, който да отпечатва на екрана "You shall not pass!". Освен това, класът има и низ (``char*``) за прякор

Напишете клас "DragonWizard", който наследява едновременно Dragon и Wizard, променя метода ``breatheFire()`` да отпечатва "rraagghh!" и метода ``castMagic()`` да отпечатва "\*zwing\*"

Методът print() трябва да дава информация за обекта, както и да извика другия/ите метод/и от класа, в който се намира.

Входните данни трябва да са валидирани. Creature без зададео име не може да съществува.\
Погрижете се паметта да е заделена и изтрита коректно във всички случаи.

Не е позволено ползването на std::string или ваш String клас.

Примерен код:
```cpp
Dragon toothless("Toothless");
Wizard gandalf("Gandalf", "The old man");
DragonWizard toothless_gandalf("Toothless Gandalf", "The old dragon man");

// one implementation of 'printCreature' (no templates)
printCreature(&toothless);
std::cout << '\n';
printCreature(&gandalf);
std::cout << '\n';
printCreature(&toothless_gandalf);
```

Примерен изход:
```
This creature is a Dragon named Toothless. RRAAGGHH!!!

This creature is a Wizard named Gandalf, a.k.a. The old man. You shall not pass!

This creature is a DragonWizard named Toothless Gandalf, a.k.a. The old dragon man. *zwing* rraagghh!
```
