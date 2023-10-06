# TestoweRepoTomasza
test123


#include <iostream>
#include <cstdlib>   // do generowania losowych liczb
#include <ctime>     // do obsługi czasu

int main() {
    // Inicjalizacja generatora liczb losowych
    std::srand(std::time(0));

    while (true) {
        // Generowanie losowej liczby od 1 do 100
        int random_number = std::rand() % 100 + 1;

        // Wyświetlenie wylosowanej liczby
        std::cout << "Wylosowana liczba: " << random_number << std::endl;

        // Oczekiwanie 3 sekundy
        std::this_thread::sleep_for(std::chrono::seconds(3));
    }

    return 0;
}
