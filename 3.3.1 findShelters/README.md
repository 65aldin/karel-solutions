# 3.3.1 findShelters

## Lösungen

```java
void findShelters() {
    repeat (4) {
        if (frontIsClear() && !beeperAhead()) {
            moveForward();
            if (leftIsClear() || frontIsClear() || rightIsClear()) {
                dropBeeper();
                findShelters();
            }
            turnAround();
            moveForward();
            turnAround();
        }
        turnLeft();
    }
}
```
