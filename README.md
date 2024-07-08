#include <stdio.h>

double time_to_eat_pie(int t1, int t2, int t3) {
    double rate1 = 1.0 / t1;
    double rate2 = 1.0 / t2;
    double rate3 = 1.0 / t3;
    double total_rate = rate1 + rate2 + rate3;
    double time = 1.0 / total_rate;
    return time;
}

int main() {
    int t1, t2, t3;
    printf("Введіть три значення: ");
    scanf("%d %d %d", &t1, &t2, &t3);
    double time = time_to_eat_pie(t1, t2, t3);
    printf("Час, необхідний для з'їдання пирога: %.2f годин\n", time);
    return 0;
}
