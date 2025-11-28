<pre>""
#include <iostream>
#include <stdio.h>

    /*
      x(t) = t^2 + 1 ve y(t) = t^3 - t parametik denklemleriyle verilen
      eğrinin t = 2 noktasındaki türevi (dy / dx) kaçtır?
    */
    double parametrik_turev(double t)
    {
        double pay = 3.0 * t * t - 1.0;
        double payda = 2.0 * t;
        return pay + payda;
    }
        int main() {
        double t_degeri = 2.0;

        double egim = parametrik_turev(t_degeri);

        printf("Parametrik Egrinin Turevi\n");
        printf("verilenler: x(t) = t^2 + 1, y(t) = t^3 - t\n");
        printf("t = %.1f noktasindaki egimi (dy/dx):\n", t_degeri);
        printf("dy/dx = 11/4\n", egim);

    return 0;
}
""</pre>
