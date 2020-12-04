package ru.gregory.java.core;
import java.util.Random;
public class Core1 {
    public static void main(String[] args) {
        Random rand = new Random(9);
        Actions[] action = new Actions[3];
        int distance = rand.nextInt(9);
        int heigth = rand.nextInt(11);
       action [0] =  new Cat("Barsik", distance, heigth);
        distance = rand.nextInt(9);
        heigth = rand.nextInt(11);
        action[1] = new Human("Gregory", distance, heigth);
        distance = rand.nextInt(9);
        heigth = rand.nextInt(11);
        action[0] =  new Robot("Terminator", distance, heigth);
        Barrier[] barriers = new Barrier[6];
        boolean isRoad;
        for (int i = 0; i < barriers.length; i++) {
            distance = rand.nextInt(10);
            isRoad = rand.nextBoolean();
            if (isRoad) {
                barriers[i] = new Barrier("Road " + i, distance);
            } else {
                barriers[i] = new Barrier("Wall " + i, distance);
            }
        }
        for (int i = 0; i < action.length; i++) {
            boolean result = true;
            for (int j = 0; j < barriers.length; j++) {
            }
        }
    }
}
