# AoC Java Executor

Java executor for the [Advent of Code Solver](https://github.com/tcollier/aoc_solver).

## Signature

```java
public interface Solution<T> {
  public String part1Answer(ArrayList<T>);
  public String part2Answer(ArrayList<T>);
}

public class Executor {
  public Executor(Solution<T> solution, ArrayList<T> input);
  public void run(String[] args);
}
```

## Template Code

```java
// Main.java
import java.util.ArrayList;

import tcollier.Executor;
import tcollier.Solution;

class Day1Solution implements Solution<String> {
  private ArrayList<String> input;

  public String part1Answer(ArrayList<String> input) {
    // compute part 1 solution
    return solution
  }

  public String part2Answer(ArrayList<String> input) {
    // compute part 2 solution
    return solution
  }
}

class Main {
  public static void main(String[] args) {
    ArrayList<String> input = // load input
    Executor executor = new Executor(new Day1Solution(), input);
    executor.run(args);
  }
}
```
