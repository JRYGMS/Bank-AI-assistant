# Bank-AI-assistant
Lekki system klasyfikacji intencji w języku naturalnym (NLP), symulujący obsługę konta bankowego. Projekt wykorzystuje sieci neuronowe do mapowania zapytań tekstowych użytkownika na konkretne akcje systemowe, takie jak zarządzanie saldem i autoryzacja transakcji.

# Kluczowe Funkcjonalności
Rozpoznawanie intencji (Intent Recognition): Klasyfikacja tekstu do jednej z trzech kategorii: zapytanie o saldo, wpłata lub wypłata.

# Przetwarzanie wstępne (Preprocessing): Wykorzystanie tokenizacji i techniki paddingu sekwencji do ujednolicenia wejścia danych tekstowych dla modelu.

# Dynamiczne zarządzanie stanem: System w czasie rzeczywistym aktualizuje wirtualne saldo konta w zależności od wyniku klasyfikacji.

# Obsługa logiki transakcyjnej: Weryfikacja dostępności środków przed wykonaniem operacji wypłaty.

# Stos technologiczny (Tech Stack)
Język: Python.

Deep Learning: TensorFlow, Keras (Sequential API).

Przetwarzanie danych: NumPy (operacje na tensorach).

Architektura modelu: Warstwa Embedding (osadzenia wektorowe), GlobalAveragePooling1D oraz warstwy gęste (Dense) z aktywacją Softmax.

# Architektura Rozwiązania
Dataset: Zbiór fraz treningowych mapowanych na etykiety numeryczne reprezentujące intencje.

Model: Sieć neuronowa trenowana przez 500 epok przy użyciu optymalizatora Adam i funkcji straty Sparse Categorical Crossentropy.

Deployment: Interfejs konsolowy działający w pętli zamkniętej, zapewniający interakcję z użytkownikiem w trybie ciągłym.
