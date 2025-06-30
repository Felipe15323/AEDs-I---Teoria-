# 📚 AEDs I - Teoria (Algoritmos e Estruturas de Dados I)

Este repositório contém materiais da disciplina **Algoritmos e Estruturas de Dados I**, cursada na UNIFAL-MG. Aqui você encontrará códigos de exemplo, anotações teóricas e implementações em **C++**.

---

## 📂 Conteúdo

### 🔹 `algoritmos_basicos/`
- Implementações simples de algoritmos como busca e ordenação

### 🔹 `estruturas/`
- Estruturas de dados clássicas: pilha, fila e listas

### 🔹 `anotações/`
- Resumos teóricos e explicações importantes

---

## 💻 Linguagem utilizada

- C++ (com uso básico de STL onde necessário)

---

> *Disciplina cursada em Ciência da Computação - UNIFAL-MG*

Exemplo de código

#include <iostream>
using namespace std;

int buscaLinear(int vetor[], int tamanho, int chave) {
    for (int i = 0; i < tamanho; i++) {
        if (vetor[i] == chave) return i;
    }
    return -1;
}

int main() {
    int v[] = {10, 20, 30, 40, 50};
    int pos = buscaLinear(v, 5, 30);
    if (pos != -1)
        cout << "Elemento encontrado na posição: " << pos << endl;
    else
        cout << "Elemento não encontrado." << endl;
    return 0;
}
