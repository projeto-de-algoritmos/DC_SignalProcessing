# Signal Processing

**Conteúdo da Disciplina**: D&C<br>

## Alunos
|Matrícula | Aluno |
| -- | -- |
| 15/0122837  |  Davi Alves Bezerra |

## Sobre 
Uma breve introdução a processamento de sinais com o uso do algoritmo fast fourier transform (FFT).
Através do jupyter notebook é possivel de forma interativa ir vizualizando o que compõe o som digital como conhecemos. Foram escolhidas para o exemplo algumas notas de piano gravadas por microfone digital, `C` `E` `F` `A` , é possivel reconhecer cada nota por sua frequencia fundamental.
### Teclas e frequências
![image](https://user-images.githubusercontent.com/34287081/209881122-8b483f5a-ab6a-43f9-832c-fa50cc900c87.png)

### Dominio da frequência com DFT
Outra representação gráfica útil é a do conteúdo da frequência, ou espectro da nota. A maneira padrão de fazer isso é com uma transformada discreta de Fourier (https://en.wikipedia.org/wiki/Discrete_Fourier_transform) usando a transformação rápida de Fourier (https://en.wikipedia.org/wiki/Fast_Fourier_transform) ou algoritmo FFT . Basicamente, pegamos um sinal sonoro e isolamos as frequências das ondas senoidais que compõem esse som.

O algoritmo "Fast Fourier Transform" é uma forma otimizada para calcular o DFT. A implementação simples da DFT faz O(n²) operações. O algoritmo Cooley-Tukey FFT clássico implementado em FFTPACK é usado pelas bibliotecas SciPy e Numpy. Inicialmente o algoritmo FFT foi usado por Gauss para determinar órbitas periódicas de asteroides, enquanto Cooley e Turkey o usaram para detectar testes nucleares soviéticos e popularizaram o algoritmo. FFT ultiliza da tecnica de dividir e conquistar para fazer a multiplicação dos polinomios com uma complexidade de tempo O(nlogn). Todo o nosso mundo digital usa esses algoritmos simples, mas realmente poderosos, que transformam sinais de seu domínio de tempo em seu domínio de frequência e vice-versa.
![image](https://user-images.githubusercontent.com/34287081/209881462-db31fd41-ff5a-4a67-ad0e-53f4ea67551a.png)
*Book: python numerical methods, berkeley*

## Instalação 
**Linguagem**: Python<br>
**Framework**: Jupyter Notebook<br>
Se preferir, use o google colab para rodar o codigo.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VnklJEZVuUgRivX_WWzVvUCe0IUI1V8e?usp=sharing)
