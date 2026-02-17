# conflict
Here’s a simple Dart program
that computes
and prints the Fibonacci sequence.
```dart
import 'dart:io';

void main() {
  stdout.write("Enter how many Fibonacci numbers to generate: ");
  int n = int.parse(stdin.readLineSync()!);

  List<int> fibonacci = generateFibonacci(n);

  print("Fibonacci sequence:");
  print(fibonacci);
}

List<int> generateFibonacci(int n) {
  if (n <= 0) return [];
  if (n == 1) return [0];

  List<int> sequence = [0, 1];

  for (int i = 2; i < n; i++) {
    sequence.add(sequence[i - 1] + sequence[i - 2]);
  }

  return sequence;
}
```
