# 1.3.1 harvestTheField

## Lösung

```java
void harvestTheField() {
    repeat (2) {
        pick();
        repeat (2) {
            moveForward();
            moveForward();
            turnLeft();
        }
        pick();
        turnAround();
    }
}

void pick() {
    repeat (4) {
        moveForward();
        pickBeeper();
        turnRight();
        moveForward();
        turnLeft();
    }
}
```
