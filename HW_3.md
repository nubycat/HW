import numpy as np
import matplotlib.pyplot as plt

# Beta-распределение
a = 2
b = 5
size = 1000
beta_dist = np.random.beta(a, b, size)
plt.hist(beta_dist, bins=30, density=True)
plt.title('Beta-распределение (a={}, b={})'.format(a, b))
plt.show()

# Биномиальное распределение
n = 10
p = 0.5
size = 1000
binomial_dist = np.random.binomial(n, p, size)
plt.hist(binomial_dist, bins=10, density=True)
plt.title('Биномиальное распределение (n={}, p={})'.format(n, p))
plt.show()

# Экспоненциальное распределение
scale = 1
size = 1000
exponential_dist = np.random.exponential(scale, size)
plt.hist(exponential_dist, bins=30, density=True)
plt.title('Экспоненциальное распределение (scale={})'.format(scale))
plt.show()

# Гамма-распределение
shape = 2
scale = 2
size = 1000
gamma_dist = np.random.gamma(shape, scale, size)
plt.hist(gamma_dist, bins=30, density=True)
plt.title('Гамма-распределение (shape={}, scale={})'.format(shape, scale))
plt.show()

# Геометрическое распределение
p = 0.3
size = 1000
geometric_dist = np.random.geometric(p, size)
plt.hist(geometric_dist, bins=10, density=True)
plt.title('Геометрическое распределение (p={})'.format(p))
plt.show()

# Нормальное распределение
loc = 0
scale = 1
size = 1000
normal_dist = np.random.normal(loc, scale, size)
plt.hist(normal_dist, bins=30, density=True)
plt.title('Нормальное распределение (loc={}, scale={})'.format(loc, scale))
plt.show()

# Пуассоновское распределение
lam = 3
size = 1000
poisson_dist = np.random.poisson(lam, size)
plt.hist(poisson_dist, bins=15, density=True)
plt.title('Пуассоновское распределение (lam={})'.format(lam))
plt.show()

# Равномерное распределение
low = 0
high = 10
size = 1000
uniform_dist = np.random.uniform(low, high, size)
plt.hist(uniform_dist, bins=20, density=True)
plt.title('Равномерное распределение (low={}, high={})'.format(low, high))
plt.show()
