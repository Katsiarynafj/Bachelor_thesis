# Bachelor_thesis
Bacterial transcripts’ codon usage optimization based on genomic tRNA gene organization
1. “transcripts_OR.ipynb”: odczytuje sekwencje transkryptów genów kodujących białka u badanych 
bakterii z plików FASTA. Oblicza prawdopodobieństwa występowania pojedynczych kodonów, ich 
par i na tej podstawie oblicza stosunek szans (OR).  
2. “tRNA_clustrers_OR.ipynb”: odczytuje listę antykodonów tRNA, które występują w klastrach w 
genomie badanych bakterii, z plików tekstowych. Oblicza prawdopodobieństwa występowania 
pojedynczych antykodonów tRNA, ich par i na tej podstawie oblicza stosunek szans (OR).  
3. “data_alignment.ipynb”: łączy wyniki analizy współczynników szans kodonów/antykodonów tRNA 
z dwóch różnych zestawów danych (z punktu 1 i 2) u wybranych bakterii.  
4. “heat_maps.ipynb”: generuje mapę ciepła współwystępowania par kodonów w sekwencjach DNA 
wybranych bakterii na podstawie danych z pliku Excel (dane z punktu 1).  
5. “codon_pair_graphs.ipynb”: generuje grafy par kodonów współwystępujących w transkryptach 
wybranych bakterii w wybranych zakresach logarytmów stosunków szans (dane z punktu 1), 
zaznaczając grubością linii wartości tych stosunków. 
6. “cereus(OR)_wobble_position_modification.ipynb”: uwzględnia wybrane modyfikacje w pozycji 
wobble w B. cereus w analizie przeprowadzonej wcześniej (punkt 1 i 2). Zakłada się, że OR kodonów 
niekomplementarnych jest równy OR kodonów komplementarnych. 
7. “codon_usage_optimalization.ipynb”: analizuje użycie kodonów w sekwencjach B. thuringiensis z 
pliku FASTA, oblicza względną częstotliwość każdego kodonu (RSCU), optymalizuje sekwencje genu 
glikoproteiny G na podstawie tych danych. Pod koniec oblicza się ilość zmienionych kodonów i 
stosunki par GC przed i po optymalizacji. 
8. “RSCU_wykres.ipynb”: generuje wykres z RSCU dla aminokwasów w sekwencjach DNA 
B.thuringiensis. 
9. “correlation_optimization.ipynb”: przyjmuje zoptymalizowaną sekwencję, otrzymaną w punkcie 7, 
oraz słownik z zamianami kodonów dla wybranych aminokwasów (S, C, H). Następnie zamienia 
każdy kodon odpowiadający zamianie zdefiniowanej w słowniku. Pod koniec oblicza się ilość 
zmienionych kodonów i stosunki par GC przed i po optymalizacji. 