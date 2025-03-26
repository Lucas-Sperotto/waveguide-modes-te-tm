# Guia de Ondas Circulares: Modos TE e TM 

Este repositório reúne códigos, visualizações e explicações sobre os modos TE (Transversal Elétrico) e TM (Transversal Magnético) em **guias de onda circulares metálicos**. O projeto integra simulações em **Python** e **C++**, com foco no cálculo das frequências de corte, distribuições de campo e uso de funções de Bessel.

---

## 📊 Objetivo

Fornecer um estudo computacional completo sobre a propagação modal em guias circulares, incluindo:

- Cálculo das **frequências de corte** para modos TE/TM
- Geração das **raízes das funções de Bessel** com SciPy
- Código C++ que utiliza as raízes para calcular as frequências
- Visualizações 2D dos campos modais
- Explicações teóricas acessíveis

---

## 🔢 Conteúdo do Repositório

### 1. `README.md`
> Visão geral do projeto

### 2. `bessel_roots_generator.py`
> Script Python que gera `bessel_roots.csv` com as raízes das funções de Bessel e suas derivadas (usado em modos TM e TE)

### 3. `calcular_frequencias_de_corte.cpp`
> Código C++ que:
> - Lê o arquivo CSV de raízes
> - Calcula as frequências de corte em GHz
> - Gera `frequencias_de_corte.csv`

### 4. `graficos_bessel.py`
> Gera gráficos das funções de Bessel \( J_0, J_1, J_2 \) e suas derivadas, com marcação das raízes

### 5. `campo_TE11_plot.py`
> Visualização 2D do campo longitudinal \( H_z \) para o modo TE<sub>11</sub>

### 6. `teoria_bessel.md`
> Explicação sobre as funções de Bessel e sua aparição nos guias de onda

### 7. `modos_degenerados.md`
> O que são modos degenerados e sua relevância física

### 8. `estrutura_campos.md`
> Derivação da equação de Helmholtz em coordenadas cilíndricas e aparecimento das soluções com Bessel

---

## 🚀 Como usar

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```

2. Gere as raízes:
```bash
pip install scipy
python3 bessel_roots_generator.py
```

3. Compile e execute o código C++:
```bash
g++ -o calcular_frequencias calcular_frequencias_de_corte.cpp
./calcular_frequencias
```

4. Execute os scripts de visualização:
```bash
python3 graficos_bessel.py
python3 campo_TE11_plot.py
```

---

## 🎓 Licença

Este projeto está licenciado sob a MIT License. Sinta-se livre para utilizar, modificar e contribuir.

---