Refactoring MonolithicAdventureGame Using SOLID Principles 
1.Project Overview 
This project is a refactored version of a monolithic adventure game, following SOLID principles to improve modularity, scalability, and maintainability.

📂 SOLID-Refactored-AdventureGame 
│── 📂 src 
│ ├── 📂 player 
│ │ ├── Player.java 
│ ├── 📂 combat 
│ │ ├── CombatManager.java 
│ ├── 📂 enemies 
│ │ ├── Enemy.java 
│ │ ├── Skeleton.java 
│ │ ├── Zombie.java 
│ │ ├── Vampire.java 
│ ├── 📂 items 
│ │ ├── ItemManager.java 
│ │ ├── GoldCoin.java 
│ │ ├── HealthElixir.java 
│ │ ├── MagicScroll.java 
│ ├── 📂 level 
│ │ ├── LevelManager.java 
│ ├── 📂 score 
│ │ ├── ScoreManager.java 
│ ├── MainGame.java 
│ │── 📂 docs 
│ ├── image diagram.docx  
│ ├── SOLID-Refactoring-Report.pdf 
│ │── README.md 
2. Applied SOLID Principles 
✅ Single Responsibility Principle (SRP) 
Each class is responsible for only one functionality (separate classes for Player, Enemy, Items, Combat, Levels, and Score). 
✅ Open/Closed Principle (OCP) 
New enemies and items can be introduced without modifying existing code (leveraging IEnemy and IItem interfaces). 
✅ Dependency Inversion Principle (DIP) 
CombatManager relies on IEnemy instead of specific enemy classes, increasing flexibility. 
✅ Liskov Substitution Principle (LSP) 
Zombie, Vampire, and Skeleton can substitute the Enemy class without affecting game functionality. 
✅ Interface Segregation Principle (ISP) 
IEnemy and IItem interfaces are split instead of using a single large interface.
