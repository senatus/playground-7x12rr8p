# Welcome!

This C++ template lets you get started quickly with a simple one-page playground.

```C++ runnable
#include <functional>
#include <iostream>

int main() {
    const std::function<std::size_t (const std::size_t)> f_fib = [&f_fib](const std::size_t v) noexcept {
        if (v <= 1)
            return v;

        return f_fib(v - 2) + f_fib(v - 1);
    };

    std::cout << f_fib(25);     // 75025
}
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C++ template](https://tech.io/select-repo/598)
