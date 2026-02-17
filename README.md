# conflict

/// User A --- Update this code

/// 0,1,1,2,3,5...

List<int> generateFibonacci(int n) {
if (n <= 0) return [];
if (n == 1) return [0];

    List<int> sequence = [0, 1];

    for (int i = 2; i < n; i++) {
    sequence.add(sequence[i - 1] + sequence[i - 2]);
    }

    return sequence;

}
