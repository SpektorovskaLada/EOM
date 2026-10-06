# 🤓 Evolutionary Optimization Methods  

🧪 Laboratory works for the **"Evolutionary Optimization Methods"** course.  

## 📦 Repository Structure
- [Lab1/ 🧬 Genetic Algorithm](./Lab1)  
  - [Lab-1EOM.ipynb](./Lab1/Lab-1EOM.ipynb) – implementation notebook  
  - [EOM_Lab1.pdf](./Lab1/EOM_Lab1.pdf) – report  

- [Lab2/ ⚖️ Multi-Objective Optimization](./Lab2)  
  - [Lab-2EOM.ipynb](./Lab2/Lab-2EOM.ipynb) – implementation notebook  
  - [EOM_Lab2.pdf](./Lab2/EOM_Lab2.pdf) – report  

- [Lab3/ 🌀 Adaptive Spiral Search](./Lab3)  
  - [Lab-3EOM.ipynb](./Lab3/Lab-3EOM.ipynb) – implementation notebook  
  - [EOM_Lab3.pdf](./Lab3/EOM_Lab3.pdf) – report  

- [README.md](./README.md) – project description

## 📌 Laboratory Works

### Laboratory Work №1️⃣
**Topic:** Investigation of the Genetic Algorithm for Optimizing Multi-Extremal Functions in Real-Valued Space  

- Implementation of a **genetic algorithm** with variations in:
  - selection methods (rank-based, tournament, random);
  - selection, crossover, and mutation parameters.
- Benchmark functions analyzed:
  - **Schwefel**
  - **Drop-Wave**
- Performance criteria: **stability, accuracy, and number of function evaluations**.  
The results demonstrated that tournament selection is prone to premature convergence, whereas rank-based and random selection methods provide superior accuracy and stability.  

---
### Laboratory Work №2️⃣  
**Topic:** Multi-Objective Optimization Using Genetic Algorithm (Pareto Dominance)  

- **Objective functions:**
  - f₁(x, y) = √((x − 1)² + (y − 7)⁴)  
  - f₂(x, y) = (x + y − 2)² + x  

- **Search space:** [-10, 10] × [-10, 10]  
- **Population size:** 200  
- **Number of generations:** 40  
- **Elitism:** 20%  
- **Crossover:** uniform  
- **Mutation:** Gaussian  

- **Four parameter configurations were evaluated:**

| Config | Selection | Crossover | Mutation | Conclusion |
|--------|-----------|-----------|----------|------------|
| No. 1  | 20%       | 70%       | 10%      | Best balance, smooth Pareto front |
| No. 2  | 10%       | 80%       | 10%      | Reduced diversity, risk of convergence |
| No. 3  | 30%       | 50%       | 20%      | Broader coverage of the front |
| No. 4  | 10%       | 30%       | 60%      | Dense front despite high mutation rate |

**Conclusion:** The baseline configuration (20/70/10) yields a stable Pareto front, while an increased mutation rate (No. 3/No. 4) provides a broader coverage of the solution space.  

---
### Laboratory Work №3️⃣ 
**Topic:** Investigation of the Adaptive Spiral Search Algorithm for Multi-Extremal Function Optimization  

- Implementation of **adaptive spiral search** with varying hyper-parameters:
  - rotation angle θ (π/6, π/3, π/4);
  - adaptation bounds (rl, ru);
  - sensitivity parameter c1.
- Benchmark functions analyzed:
  - **Schwefel**
  - **Drop-Wave**
- Performance criteria: **mean distance to the global minimum, stability, and number of function evaluations**.  
The results showed high efficiency for the Drop-Wave function but a strong tendency toward premature convergence for the Schwefel function.

## 📖 Libraries Used
- numpy
- pandas
- matplotlib
- random
- copy
- openpyxl (for Excel export)
